# Lab 21 — Phân tích rủi ro AI qua case study thực tế

- Họ và tên: Vũ Quốc Bảo
- MSSV / mã học viên: 2A202602829
- Lớp: Track1 - H201
- Ngành đã chọn: HR / tuyển dụng

### 1. Industry Risk Snapshot

| Nội dung | Đánh giá của tôi và lý do |
| --- | --- |
| Những tác hại chính có thể xảy ra | Ứng viên bị loại bất công vì tuổi, giới tính, chủng tộc hoặc khuyết tật, dẫn đến mất cơ hội việc làm và kiếm thêm thu nhập. Nhà tuyển dụng và nhà cung cấp phần mềm phải chịu ảnh hưởng rủi ro pháp lý. |
| Mức độ high-stakes | Cao. Quyết định tuyển dụng có ảnh hưởng trực tiếp đến thu nhập và sự nghiệp của ứng viên, hồ sơ bị loại ở bước lọc đầu có thể không được rà soát lại. Nhận định: ứng viên thường khó biết bản thân bị loại vì lý do gì nên khó phản đối. |
| Dữ liệu nhạy cảm có thể được sử dụng | Họ tên, ngày sinh hoặc tuổi, giới tính, ảnh, địa chỉ, trường học và năm tốt nghiệp, lịch sử làm việc, khoảng trống trong CV, thông tin có thể liên quan đến sức khỏe hoặc khuyết tật. |
| Nhu cầu human review | Cao. Nhân sự và pháp chế/tuân thủ cần xem lại hồ sơ bị AI loại, kiểm tra tỷ lệ được chọn theo nhóm định kỳ, và quyết định tuyển cuối cùng phải do người. Cả ba case dưới đều là lỗi ở bước lọc tự động. |

### 2. Case study 1 — iTutorGroup tự động loại ứng viên lớn tuổi (EEOC, 2023)

#### Brief Case

- Tổ chức / sản phẩm AI: iTutorGroup - một tập đoàn giáo dục trực tuyến toàn cầu, được thành lập vào năm 1998 bởi Eric Yang tại Thượng Hải, Trung Quốc.
- Thời gian, địa điểm / bối cảnh: Mỹ, hồ sơ tháng 3–4/2020; EEOC khởi kiện, hòa giải tháng 8/2023.
- AI được dùng để làm gì: tự động xét hồ sơ ứng viên gia sư.
- Vấn đề hoặc sự kiện đáng chú ý: EEOC cáo buộc phần mềm được lập trình để tự động loại nữ từ 55 tuổi và nam từ 60 tuổi. Công ty phủ nhận sai phạm.
- Số liệu có nguồn: hơn 200 ứng viên đủ điều kiện bị loại vì tuổi, hòa giải 365.000 USD (EEOC, 11/09/2023).
- Nguồn:
  - Greenberg Traurig - EEOC Secures First Workplace AI Settlement - 08/2023 - https://www.gtlaw.com/en/insights/2023/8/eeoc-secures-first-workplace-artificial-intelligence-settlement
- Phân biệt bằng chứng và nhận định:
  - Nguồn xác nhận cáo buộc và khoản hòa giải, không có phán quyết rằng công ty vi phạm.
  - Nhận định: đây nhiều khả năng là quy tắc lọc cứng, không phải mô hình học máy.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Ứng viên gia sư nộp hồ sơ và phần mềm tự động loại ngay, trước khi có người xem, dựa trên tuổi và giới tính. |
| Stakeholder bị ảnh hưởng | Ứng viên nữ từ 55 tuổi và nam từ 60 tuổi ở Mỹ; iTutorGroup (rủi ro pháp lý); EEOC. |
| Failure mode | Bias / fairness: kết quả bất lợi cho nhóm lớn tuổi. |
| Layer bắt đầu lỗi | Chưa đủ bằng chứng. Giả thuyết của tôi: Grounding (tiêu chí lọc cài sẵn dùng tuổi và giới) và thiếu Safety (không có người kiểm tra trước khi loại). |
| Harm xảy ra là gì? | Ứng viên lớn tuổi bị mất cơ hội được xét việc khi phần mềm tự động loại hồ sơ vì tuổi. Theo cáo buộc của EEOC thì đã xảy ra; công ty phủ nhận và vụ việc kết thúc bằng hòa giải. |
| Harm lens | Opportunity loss (mất cơ hội). |
| Severity | High |
| Scale | Medium: hơn 200 ứng viên đủ điều kiện bị loại (EEOC), trong một công ty. |
| Probability | High trong cấu hình bị cáo buộc: theo cáo buộc, ứng viên thuộc nhóm tuổi này đều bị loại tự động. Đây là đánh giá của tôi dựa trên cáo buộc. |
| Frequency | Chưa đủ dữ liệu để đánh giá ngoài giai đoạn tháng 3–4/2020 nêu trong thỏa thuận. |
| Vì sao? | Severity cao vì ứng viên bị từ chối việc làm theo tuổi và giới. Scale ở mức vừa vì chỉ một công ty và hơn 200 người. Toàn bộ dựa trên cáo buộc của EEOC và hòa giải, không phải phán quyết của tòa. |

### 3. Case study 2 — Mobley kiện Workday: AI sàng lọc ứng viên bị cáo buộc thiên lệch tuổi (Mỹ, 2023 đến nay)

#### Brief Case

- Tổ chức / sản phẩm AI: Workday - công cụ AI chấm điểm, sàng lọc ứng viên (gồm HiredScore).
- Thời gian, địa điểm / bối cảnh: Tòa liên bang quận Bắc California, kiện từ 2023 và đang tiếp diễn; tháng 5/2025 tòa công nhận sơ bộ vụ kiện tập thể theo luật chống phân biệt tuổi (ADEA).
- AI được dùng để làm gì: chấm điểm, xếp hạng, sàng lọc hồ sơ cho các nhà tuyển dụng dùng nền tảng Workday.
- Vấn đề hoặc sự kiện đáng chú ý: Mobley (trên 40 tuổi) cáo buộc công cụ gây bất lợi cho người lớn tuổi. Workday cho rằng vụ kiện thiếu căn cứ.
- Số liệu có nguồn: hơn 100 đơn xin việc bị từ chối (lời nguyên đơn), nhóm kiện gồm ứng viên từ 40 tuổi bị từ chối qua nền tảng Workday từ 24/09/2020 (Holland & Knight, 27/05/2025).
- Nguồn:
  - Holland & Knight - Federal Court Allows Collective Action Lawsuit Over Alleged AI Hiring Bias - 27/05/2025 - https://www.hklaw.com/en/insights/publications/2025/05/federal-court-allows-collective-action-lawsuit-over-alleged
  - Tòa liên bang quận Bắc California - Order re HiredScore Dispute - 29/07/2025 - https://storage.courtlistener.com/recap/gov.uscourts.cand.408645/gov.uscourts.cand.408645.158.0.pdf
  - Akin Gump - AI Law & Regulation Tracker - 29/04/2026 - https://www.akingump.com/en/insights/ai-law-and-regulation-tracker/court-allows-discrimination-claims-against-ai-hiring-tool-to-proceed-or-mobley-v-workday-inc
- Phân biệt bằng chứng và nhận định: Nguồn xác nhận các quyết định thủ tục của tòa. Việc công cụ thực sự thiên lệch vẫn là cáo buộc, chưa có phán quyết cuối cùng.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Ngay sau khi nộp đơn, công cụ AI chấm điểm, xếp hạng hoặc sàng lọc hồ sơ trước khi nhà tuyển dụng xem. |
| Stakeholder bị ảnh hưởng | Ứng viên từ 40 tuổi trở lên (Mobley và nhóm kiện); nhà tuyển dụng dùng Workday; Workday (rủi ro pháp lý). |
| Failure mode | Bias / fairness (theo cáo buộc). Có thể kèm Over-reliance: tòa chấp nhận khả năng Workday là "đại diện" của nhà tuyển dụng vì khách hàng có thể đã giao việc loại và đẩy ứng viên cho công cụ (Akin Gump). |
| Layer bắt đầu lỗi | Chưa đủ bằng chứng vì cách công cụ vận hành chưa được công bố. Giả thuyết của tôi: Model (dữ liệu huấn luyện hoặc tiêu chí chấm) và thiếu Safety (không có kiểm toán thiên lệch). |
| Harm xảy ra là gì? | Ứng viên từ 40 tuổi bị mất cơ hội việc làm khi công cụ AI bị cáo buộc chấm thấp hoặc loại hồ sơ. Hiện là cáo buộc, chưa có phán quyết, nên tôi coi là nguy cơ chưa được xác nhận. |
| Harm lens | Opportunity loss (mất cơ hội). |
| Severity | High |
| Scale | High (đánh giá của tôi): tòa công nhận sơ bộ nhóm kiện toàn nước Mỹ gồm ứng viên từ 40 tuổi bị từ chối qua Workday từ 24/09/2020. Chưa có số người bị ảnh hưởng đã được xác minh. |
| Probability | Chưa đủ dữ liệu để đánh giá: chưa có kết luận về việc công cụ có thiên lệch hay không. |
| Frequency | Chưa đủ dữ liệu để đánh giá. Mobley nêu hơn 100 đơn bị từ chối, nhưng đó là lời nguyên đơn về một người. |
| Vì sao? | Severity cao vì ảnh hưởng thu nhập và cơ hội nghề nghiệp. Scale đánh giá theo phạm vi nhóm kiện do tòa xác định, không phải số người đã chứng minh bị hại. Probability và Frequency để trống vì nguồn chỉ xác nhận tiến trình tố tụng, không có số đo thiên lệch. |

### 4. Case study 3 — Nghiên cứu University of Washington: LLM xếp hạng CV thiên lệch theo tên (2024)
 
#### Brief Case
 
- Tổ chức / sản phẩm AI: nhóm nghiên cứu University of Washington; ba LLM mã nguồn mở của Mistral AI, Salesforce và Contextual AI.
- Thời gian, địa điểm / bối cảnh: trình bày 22/10/2024 tại hội nghị AIES (San Jose). Đây là thí nghiệm có kiểm soát, không phải hệ thống tuyển dụng đang chạy thật.
- AI được dùng để làm gì: xếp hạng CV theo mức phù hợp với mô tả công việc.
- Vấn đề hoặc sự kiện đáng chú ý: giữ nguyên nội dung CV, chỉ đổi tên ứng viên (120 tên gắn với người da trắng/da đen, nam/nữ); mô hình thiên lệch rõ theo chủng tộc và giới tính.
- Số liệu có nguồn: hơn 550 CV, hơn 500 mô tả công việc, hơn 3 triệu lượt so sánh; tên gắn với người da trắng được ưu tiên 85% so với 9% với tên gắn với người da đen; tên nam 52% so với nữ 11%; tên nam da đen không bao giờ được ưu tiên hơn tên nam da trắng.
- Nguồn:
  - UW News - AI tools show biases in ranking job applicants' names according to perceived race and gender - 31/10/2024 - https://www.washington.edu/news/2024/10/31/ai-bias-resume-screening-race-gender/
- Phân biệt bằng chứng và nhận định: Nguồn xác nhận số liệu trong điều kiện thí nghiệm. Chưa có ứng viên thật bị loại, nên tác hại là nguy cơ; không thể kết luận một sản phẩm thương mại cụ thể mắc lỗi tương tự.
#### Harm Map Worksheet
 
| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Nhà tuyển dụng dùng LLM xếp hạng CV so với mô tả công việc để chọn ai được đi tiếp vòng sau. |
| Stakeholder bị ảnh hưởng | Ứng viên da đen và ứng viên nữ (nặng nhất với nam da đen); nhà tuyển dụng dùng LLM để sàng lọc. |
| Failure mode | Bias / fairness: xếp hạng khác nhau chỉ vì tên ứng viên. |
| Layer bắt đầu lỗi | Model: nhóm nghiên cứu chỉ đổi tên mà giữ nguyên nội dung CV nhưng thứ hạng vẫn đổi, nên nguồn lỗi nằm ở hành vi của mô hình. Chưa kiểm tra các lớp khác của hệ thống thật. |
| Harm xảy ra là gì? | Ứng viên da đen và nữ có nguy cơ bị xếp thấp hoặc loại khi LLM xếp hạng CV thiên lệch theo tên. Mới là nguy cơ từ thí nghiệm, chưa có ứng viên thật bị loại. |
| Harm lens | Opportunity loss (mất cơ hội). |
| Severity | High nếu được dùng thật: ảnh hưởng trực tiếp đến cơ hội việc làm. |
| Scale | Chưa đủ dữ liệu để đánh giá ngoài thực tế. Trong thí nghiệm: ba mô hình, hơn 3 triệu lượt so sánh. |
| Probability | Trong thí nghiệm: tên gắn với người da trắng được ưu tiên 85% so với 9% (da đen). Ngoài thực tế chưa đủ dữ liệu, vì hệ thống thương mại thường độc quyền. |
| Frequency | Trong thí nghiệm, xu hướng lặp lại trên hơn 3 triệu lượt so sánh. Tần suất ngoài thực tế chưa đủ dữ liệu để đánh giá. |
| Vì sao? | Số liệu lấy từ thí nghiệm có kiểm soát nên chứng minh được mô hình có thiên lệch nhưng chưa chứng minh có ứng viên thật bị hại. Severity đánh giá theo hậu quả nếu triển khai thật. |
