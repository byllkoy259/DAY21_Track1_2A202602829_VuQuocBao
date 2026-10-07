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
| High-risk moment | [Tình huống cụ thể có rủi ro] |
| Stakeholder bị ảnh hưởng | [Người dùng và các bên liên quan] |
| Failure mode | [Kiểu lỗi AI] |
| Layer bắt đầu lỗi | [UX / Grounding / Safety / Model; giải thích hoặc ghi chưa đủ bằng chứng] |
| Harm xảy ra là gì? | [Ai bị ảnh hưởng + hậu quả; ghi rõ đã xảy ra hay mới là nguy cơ] |
| Harm lens | [Loại tác hại] |
| Severity | [Low / Medium / High / Critical] |
| Scale | [Quy mô tác động và căn cứ] |
| Probability | [Khả năng xảy ra và căn cứ] |
| Frequency | [Tần suất và căn cứ] |
| Vì sao? | [Lý do cho các đánh giá; nguồn hoặc giới hạn bằng chứng] |

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
| High-risk moment | [Điền] |
| Stakeholder bị ảnh hưởng | [Điền] |
| Failure mode | [Điền] |
| Layer bắt đầu lỗi | [Điền] |
| Harm xảy ra là gì? | [Điền; phân biệt hậu quả đã xảy ra với nguy cơ] |
| Harm lens | [Điền] |
| Severity | [Điền] |
| Scale | [Điền] |
| Probability | [Điền] |
| Frequency | [Điền] |
| Vì sao? | [Điền căn cứ và giới hạn bằng chứng] |

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
| High-risk moment | [Điền] |
| Stakeholder bị ảnh hưởng | [Điền] |
| Failure mode | [Điền] |
| Layer bắt đầu lỗi | [Điền] |
| Harm xảy ra là gì? | [Điền] |
| Harm lens | [Điền] |
| Severity | [Điền] |
| Scale | [Điền] |
| Probability | [Điền] |
| Frequency | [Điền] |
| Vì sao? | [Điền] |
