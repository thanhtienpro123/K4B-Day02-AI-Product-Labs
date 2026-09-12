# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Nguyễn Thành Tiến
- Mã học viên:2A202603003
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên sắp tốt nghiệp
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 |Lặp lại |Làm 1 report bằng excel về báo cáo tài chính |nhân viên phân tích dữ liệu |Cùng 1 dạng báo cáo nhưng phải phân tích cơ bản từng cái thủ công, thời gian mất hơn 5 tiếng |
| 2 |Lặp lại |Kiểm tra và đối chiếu dữ liệu giữa 2–3 hệ thống  và có sai sót con người  |Accountant |2-15 phút cho từng tài khoản thủ công|
| 3 |Pain từ người khác |Người ở trọ hỏi lại cùng 1 câu hỏi trong bộ quy định|Chủ nhà cho thuê |Số câu hỏi về quy định chiếm hơn 70%|
| 4 |Lặp lại |Kiểm tra tình trạng trạm sạc trước khi đến nhưng thông tin không cập nhật kịp thời |Tài xế xe điện |Tới nơi mới biết trạm lỗi |
| 5 |Lặp lại |Mỗi cuộc họp phải gửi email mời đến nhiều bên liên quan, sau đó theo dõi phản hồi và nhắc những người chưa xác nhận |Nhân viên điều phối |10–30 người/cuộc họp; 5–10 cuộc họp/tuần; mỗi email mất ~1–2 phút để kiểm tra/chỉnh sửa/gửi |
| 6 |AI có thể tốt hơn |Đọc và tóm tắt nhiều feedback/comment để tìm ra các vấn đề chính |Marketing |Có thể phải xử lý 50–200 feedbacks, nếu đọc thủ công sẽ mất nhiều giờ để phân loại và tổng hợp |
| 7 | | | | |
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Gửi số lượng lớn email mời họp và theo dõi phản hồi|Có thể tìm metric đo lường hiệu quả dễ dàng sau khi dùng AI, nhu cầu và hiệu quả cao khi số lượng người dùng càng nhiều  |Chưa đo chính xác tỷ lệ người không phản hồi và tổng thời gian follow-up |
| 2 |Làm report tài chính bằng Excel thủ công |Mất hơn 5 tiếng/report; workflow rõ; có nhiều bước lặp lại; impact trực tiếp lên thời gian của analyst |cần xác định được phần nào nên được AI can thiệp |
| 3 |Kiểm tra tình trạng trạm sạc nhưng thông tin không cập nhật kịp thời |Pain chung của tài xế, có thể ảnh hưởng cả hệ thống xe điện nói chung khi gặp lỗi trên diện rộng |Chi phí lắp đặt để tạo hệ thống AI và duy trì có lớn hơn chi phí khi gặp lỗi không  |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu:Nhân viên phân tích phải thực hiện nhiều bước xử lý và phân tích thủ công trong Excel để tạo một report tài chính, mất hơn 5 tiếng/report.

Actor:Nhân viên phân tích dữ liệu

Thời điểm / bối cảnh:Khi cần lập báo cáo tài chính định kỳ hoặc phân tích một bộ dữ liệu có cấu trúc tương tự các kỳ trước

Current workflow 3-7 bước:
1. Thu thập dữ liệu. 
2. Kiểm tra và làm sạch dữ liệu. 
3. Nhập/copy dữ liệu vào Excel. 
4. Tính toán các chỉ tiêu tài chính. 
5. Phân tích biến động từng chỉ tiêu. 
6. Tạo bảng/chart. 
7. Tổng hợp thành report cuối cùng.

Bottleneck:Phân tích từng chỉ tiêu và kiểm tra kết quả thủ công. Các bước tính toán và nhận xét lặp lại giữa các kỳ báo cáo. 

Impact:
Một report mất hơn 5 tiếng. Nếu thực hiện nhiều report trong tháng/tuần, thời gian dành cho các thao tác lặp lại chiếm tỷ trọng lớn.

Success metric:
- Giảm thời gian tạo report từ >5 giờ xuống <2 giờ. 
- Giảm số thao tác Excel thủ công. 
- Giảm số lỗi trong công thức/dữ liệu. 
- Analyst dành nhiều thời gian hơn cho việc kiểm tra insight.

Non-AI alternative:

AI hypothesis:
AI có thể tự động kiểm tra dữ liệu, tính các chỉ số, phát hiện biến động bất thường và tạo draft nhận xét cho từng chỉ tiêu.
Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — ___ phút

CURRENT STATE — khoảng 30–90 phút/cuộc họp [Xác định người tham dự: 5–10'] 
↓ 
[Kiểm tra/chọn lịch: 10–20'] 
↓ 
[Soạn + chỉnh email: 5–15'] 
↓ 
[Gửi 10–30 email: 10–30'] 
↓ 
[Kiểm tra phản hồi: 5–15'] 
↓ 
[Nhắc người chưa phản hồi: 5–15'] <-- BOTTLENECK
FUTURE STATE — khoảng 10–30 phút/cuộc họp [Nhập meeting + danh sách người tham dự: 2–5']
↓ 
 [AI tạo email + đề xuất lịch: 2–5'] 
↓ 
[Human review: 2–5'] 
↓ 
[AI gửi/follow-up người chưa xác nhận: tự động]  <-- human boundary

Fallback: nếu AI sai thì Nếu AI xác định sai người nhận hoặc lịch không chính xác, hệ thống không gửi tự động mà chuyển sang trạng thái "Need human approval".
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu: 
Nhân viên phân tích phải thực hiện nhiều bước xử lý và phân tích thủ công trong Excel để tạo một report tài chính, mất hơn 5 tiếng/report. 

Actor: Nhân viên phân tích dữ liệu / Financial Analyst.

Thời điểm / bối cảnh: Khi cần lập báo cáo tài chính định kỳ hoặc phân tích một bộ dữ liệu có cấu trúc tương tự các kỳ trước. 

Current workflow 3-7 bước: 1. Thu thập dữ liệu. 2. Kiểm tra và làm sạch dữ liệu. 3. Nhập/copy dữ liệu vào Excel. 4. Tính toán các chỉ tiêu tài chính. 5. Phân tích biến động từng chỉ tiêu. 6. Tạo bảng/chart. 7. Tổng hợp thành report cuối cùng. 
Bottleneck: Phân tích từng chỉ tiêu và kiểm tra kết quả thủ công. Các bước tính toán và nhận xét lặp lại giữa các kỳ báo cáo. Impact: Một report mất hơn 5 tiếng. Nếu thực hiện nhiều report trong tháng/tuần, thời gian dành cho các thao tác lặp lại chiếm tỷ trọng lớn. 
Success metric: 
- Giảm thời gian tạo report từ >5 giờ xuống <2 giờ.
- Giảm số thao tác Excel thủ công. 
- Giảm số lỗi trong công thức/dữ liệu. 
- Analyst dành nhiều thời gian hơn cho việc kiểm tra insight. 
Non-AI alternative: Excel template + Power Query + Pivot Table + VBA/macros. 
AI hypothesis: AI có thể tự động kiểm tra dữ liệu, tính các chỉ số, phát hiện biến động bất thường và tạo draft nhận xét cho từng chỉ tiêu.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — >300 phút/report 
[Thu thập dữ liệu: 30'] 
↓ 
[Clean dữ liệu: 45']
↓ 
[Copy/import vào Excel: 30'] 
↓ 
[Tính toán chỉ tiêu: 60'] 
↓ 
[Phân tích từng chỉ tiêu: 90'] <-- BOTTLENECK 
↓ 
[Chart + formatting: 30'] 
↓ 
[Review: 15'] 
FUTURE STATE 
— khoảng 90–120 phút/report [Upload dữ liệu: 5'] 
↓ 
[AI kiểm tra + clean: 15'] 
↓ 
[AI tính toán + phát hiện biến động: 15'] 
↓ 
[AI tạo draft insight: 10'] 
↓ 
[Human review + chỉnh insight: 30–60'] <-- HUMAN BOUNDARY 
↓ 
[Export report: 10']
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu: Tài xế xe điện không luôn nhận được thông tin chính xác và kịp thời về tình trạng hoạt động/bảo trì của trạm sạc trước khi đến.

Actor: Tài xế xe điện.

Thời điểm / bối cảnh:
Khi tài xế cần tìm trạm sạc và quyết định trạm nào sẽ đến.

Current workflow 3-7 bước:
1. Mở ứng dụng/bản đồ để tìm trạm sạc. 
2. Kiểm tra tình trạng trạm. 
3. Chọn trạm dựa trên thông tin hiển thị. 
4. Di chuyển đến trạm. 
5. Đến nơi và kiểm tra thực tế. 
6. Nếu trạm lỗi/bảo trì thì tìm trạm khác. 
7. Thay đổi lộ trình và tiếp tục di chuyển.

Bottleneck: Thông tin trạng thái trạm không được cập nhật kịp thời. Tài xế chỉ phát hiện vấn đề sau khi đã đến nơi.

Impact: Tài xế có thể mất thêm thời gian di chuyển, phải chờ hoặc tìm một trạm khác. Trải nghiệm sử dụng xe điện bị ảnh hưởng.

Success metric: 
- Tăng độ chính xác của trạng thái trạm. 
- Giảm số trường hợp tài xế đến trạm nhưng không thể sạc.
- Giảm thời gian tìm trạm thay thế. 
- Giảm quãng đường đi thêm do trạm không hoạt động.

Non-AI alternative:
Thiết lập quy trình cập nhật trạng thái trạm theo thời gian thực và đồng bộ dữ liệu giữa hệ thống vận hành và ứng dụng tài xế.

AI hypothesis:
AI có thể tổng hợp dữ liệu từ hệ thống vận hành, lịch bảo trì và phản hồi của tài xế để dự đoán/cảnh báo khả năng trạm không hoạt động và đề xuất trạm thay thế.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE 
— khoảng 20–40 phút [Mở app tìm trạm: 2'] 
↓ 
[Kiểm tra trạng thái: 2–5'] 
↓ 
[Chọn trạm: 2–5'] 
↓ 
[Di chuyển đến trạm: 10–20'] 
↓ 
[Phát hiện trạm lỗi/bảo trì: 2–5'] <-- BOTTLENECK 
↓ 
[Tìm trạm khác: 5–15'] 
↓ 
[Di chuyển lại: 5–20'] FUTURE STATE 
— khoảng 10–25 phút [Nhập nhu cầu sạc: 1'] 
↓ 
[AI kiểm tra trạng thái + dữ liệu bảo trì: tự động] 
↓ 
[AI đánh giá khả năng sạc thành công: <1'] 
↓ 
[Đề xuất trạm phù hợp: 1'] 
↓ 
[Human/tài xế review lựa chọn: 1–2'] 
↓ 
[Di chuyển trực tiếp đến trạm phù hợp]

Fallback: Nếu dữ liệu trạng thái không đủ hoặc AI confidence thấp, hiển thị nhiều lựa chọn trạm và cảnh báo: "Thông tin trạng thái chưa được xác nhận gần đây".
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Workflow hiện tại là tài xế chọn trạm → di chuyển đến trạm → đến nơi mới biết trạm đang đông/bảo trì → phải chờ hoặc tìm trạm khác. Mỗi lần gặp tình trạng này có thể làm tài xế mất thêm 15–30 phút hoặc hơn, đồng thời tăng quãng đường di chuyển và nguy cơ không đủ pin để tiếp tục hành trình. Đây là vấn đề lặp lại, có impact trực tiếp đến thời gian, chi phí và trải nghiệm của tài xế.

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Liệu vấn đề chính là không biết trạm đang hoạt động, hay quan trọng hơn là không biết khi mình đến thì trạm còn chỗ hay phải chờ bao lâu?
Nếu các app đã có thông tin trạng thái trạm, liệu AI có thực sự tạo thêm giá trị bằng cách dự đoán tình trạng trạm tại thời điểm tài xế đến không?

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Thông tin “trạm đông/bảo trì” có thể đã được một số ứng dụng cập nhật, nên nếu chỉ xây dựng tính năng hiển thị Available/Unavailable thì chưa đủ khác biệt và chưa cần AI.

```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Thông tin “trạm đông/bảo trì” có thể đã được một số ứng dụng cập nhật, nên nếu chỉ xây dựng tính năng hiển thị Available/Unavailable thì chưa đủ khác biệt và chưa cần AI.
- Tôi sửa gì: Chuyển trọng tâm từ “trạm hiện tại có hoạt động không?” sang “khi tài xế đến, trạm có còn khả năng sạc và phải chờ bao lâu?”. AI sẽ kết hợp trạng thái realtime + số cổng đang sử dụng + lịch sử nhu cầu + ETA của tài xế để dự đoán mức độ đông và thời gian chờ, sau đó đề xuất trạm thay thế nếu thời gian chờ quá lâu.

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
