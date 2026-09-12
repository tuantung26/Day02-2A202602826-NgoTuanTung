# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Ngô Tuấn Tùng
- Mã học viên: 2A202602826
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm 2, Intern AI Engineer.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
    - Các công việc freelance ở công ty.
    - Công việc cá nhân.
    - Việc học tập hằng tuần.
    - Dạy thêm bên ngoài.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại | Mỗi tuần phải tìm lại tài liệu, code và notebook cũ để tiếp tục một bài AI/ML | Tôi | Khoảng 20-30 phút/lần, khoảng 3 lần/tuần |
| 2 | Tốn thời gian | Đọc nhiều tài liệu/paper để tìm đúng phần liên quan đến bài đang làm | Tôi | Khoảng 30-60 phút/lần, khoảng 2-3 lần/tuần |
| 3 | Tốn thời gian | Debug lỗi code AI nhưng phải tự tìm từ traceback, Google và các đoạn code cũ | Tôi | Khoảng 30-90 phút/lỗi, thường 2-3 lỗi/tuần |
| 4 | Lặp lại | Chuẩn bị môi trường và chạy lại code train/test model nhiều lần | Tôi | Khoảng 15-30 phút/lần, khoảng 2-4 lần/tuần |
| 5 | AI có thể tốt hơn | Có nhiều paper hoặc tài liệu nhưng khó nhanh chóng biết paper nào đáng đọc trước | Tôi | Mỗi lần tìm tài liệu thường mở khoảng 5-10 nguồn trước khi chọn |
| 6 | AI có thể tốt hơn | Khi học một kiến thức mới về AI, phải đọc nhiều nguồn rồi tự ghép lại thành cách hiểu của mình | Tôi | Khoảng 30-60 phút/chủ đề, khoảng 2 lần/tuần |
| 7 | Pain từ người khác | Khi dạy thêm, học viên hay hỏi lại những phần đã giải thích nhưng theo cách khác | Học viên và tôi | Khoảng 2-5 câu hỏi lặp lại/buổi dạy |
| 8 | Tốn thời gian | Chuẩn bị nội dung và bài tập trước khi dạy thêm | Tôi | Khoảng 30-60 phút/buổi, khoảng 2-3 buổi/tuần |
| 9 | Lặp lại | Chuyển nội dung học hoặc công việc thành note để sau này dễ tìm lại | Tôi | Khoảng 15-30 phút/lần, khoảng 2-3 lần/tuần |
| 10 | Pain từ người khác | Khi làm freelance, yêu cầu công việc đôi khi chưa rõ nên phải hỏi lại để biết chính xác cần làm gì | Tôi và người giao việc | Khoảng 1-3 lần hỏi lại/task, gặp khoảng 1-2 task/tuần |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: "Dựa trên vai trò sinh viên năm 2 và Intern AI Engineer, hãy gợi ý các problem có thể quan sát được trong việc học AI, làm freelance, làm project và dạy thêm. Ưu tiên problem lặp lại, tốn thời gian và có thể đo bằng thời gian hoặc số lần."
- Ý dùng được: Gợi ý thêm các vấn đề về tìm tài liệu, debug code, chuẩn bị môi trường, ghi chú và chuẩn bị bài dạy.
- Ý bỏ vì không phải pain thật: Bỏ các ý quá lớn như "AI giúp nghiên cứu AI tốt hơn" hoặc "xây agent tự động làm project", vì chưa có workflow và số liệu rõ ràng.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Debug lỗi code AI nhưng phải tự tìm từ traceback, Google và các đoạn code cũ | Xảy ra khá thường xuyên; mỗi lỗi có thể mất 30-90 phút; workflow từ đọc lỗi đến sửa code khá rõ | Chưa đo chính xác thời gian trung bình cho từng loại lỗi |
| 2 | Đọc nhiều tài liệu/paper để tìm đúng phần liên quan đến bài đang làm | Liên quan trực tiếp đến việc học và nghiên cứu AI; mất khá nhiều thời gian; có thể đo số tài liệu và thời gian đọc | Chưa chắc AI giúp giảm thời gian mà vẫn tìm đúng tài liệu |
| 3 | Chuẩn bị nội dung và bài tập trước khi dạy thêm | Lặp lại hằng tuần; workflow rõ; có thể đo thời gian chuẩn bị và thời gian sửa bài | Chưa chắc phần nào AI làm tốt, phần nào nên tự làm |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Debug lỗi code AI

```text
Problem 1 câu: Mỗi khi code AI bị lỗi, tôi phải đọc traceback, tìm nguyên nhân trên mạng và thử sửa nhiều lần nên có lỗi mất từ 30-90 phút mới xử lý xong.

Actor: Tôi - sinh viên năm 2 và Intern AI Engineer.

Thời điểm / bối cảnh: Khi làm project AI/ML, train model hoặc chạy thử code.

Current workflow 3-7 bước:
1. Chạy code và gặp lỗi.
2. Đọc traceback để xem lỗi nằm ở đâu.
3. Tìm lỗi trên Google/GitHub/Stack Overflow.
4. Đọc các kết quả và thử cách sửa.
5. Chạy lại code.
6. Nếu vẫn lỗi thì quay lại tìm tiếp.

Bottleneck: Bước 3-4 - tìm đúng nguyên nhân và cách sửa, vì có nhiều kết quả khác nhau và phải tự kiểm tra từng cách.

Impact: Mỗi lỗi mất khoảng 30-90 phút. Trung bình có khoảng 2-3 lỗi/tuần khi làm project hoặc học.

Success metric: Giảm thời gian xử lý một lỗi từ khoảng 30-90 phút xuống dưới 20 phút, nhưng code sau khi sửa vẫn chạy đúng.

Non-AI alternative: Viết checklist debug, lưu lại các lỗi đã gặp và tạo thư viện các lỗi thường gặp.

AI hypothesis: AI đọc traceback, đoạn code liên quan và giải thích nguyên nhân, sau đó gợi ý cách sửa. Tôi vẫn kiểm tra và chạy lại code.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
