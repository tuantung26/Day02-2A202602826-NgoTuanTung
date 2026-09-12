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
| 1 | Lặp lại | Soạn bài tập trắc nghiệm cho học sinh dạy thêm. | Bản thân, học sinh | Mất 2 tiếng/tuần để bịa và gõ 30 câu hỏi, tuần nào cũng phải làm. |
| 2 | Tốn thời gian | Đọc và tóm tắt các paper/tài liệu chuyên ngành dài ngoằng cho task intern. | Bản thân | Mất 3-4 tiếng/tuần đọc 2-3 paper (10-15 trang/bản) nhưng chỉ chắt lọc được 1-2 ý dùng được. |
| 3 | AI có thể tốt hơn | Viết các đoạn code tiền xử lý dữ liệu (data cleaning) cơ bản. | Bản thân | Lặp lại 3-4 lần/tuần, mỗi lần mất 30-45 phút gõ mấy hàm pandas quen thuộc. |
| 4 | Pain từ người khác | Học sinh nhắn tin hỏi bài cũ, hỏi các bài tập cơ bản vào buổi tối. | Bản thân, học sinh | Nhận 10-15 tin nhắn/tuần vào buổi tối, mất 45 phút gõ text giải thích từng bước trên điện thoại. |
| 5 | Tốn thời gian | Gom nhặt hóa đơn, chi tiêu từ Momo/Banking để ghi chép vào file quản lý tài chính cá nhân. | Bản thân | Mất 1 tiếng/tuần vào tối Chủ nhật để dò lại lịch sử giao dịch và nhập tay vào Notion. |
| 6 | Lặp lại | Viết email báo cáo tiến độ (Weekly Report) cho anh Mentor ở công ty. | Bản thân, Mentor | Mất 30 phút chiều thứ 6 hàng tuần để nhớ lại xem tuần này làm được những gì rồi gõ thành gạch đầu dòng. |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Có thể gợi ý cho sinh viên năm 2 kiêm intern AI một số việc nhàm chán lặp lại không?
- Ý dùng được: Chuyện viết code boilerplate data cleaning.
- Ý bỏ vì không phải pain thật: AI bảo tự động hóa việc đi học trên trường (cái này bắt buộc phải lên lớp điểm danh nên không làm được).

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
| 1 | Soạn bài tập trắc nghiệm cho học sinh dạy thêm. | Tốn nhiều thời gian cuối tuần nhất, rất nhàm chán; Đầu ra rõ ràng (text, câu hỏi). | Sợ AI bịa kiến thức sai (hallucination) trong đáp án các môn tự nhiên. |
| 2 | Đọc và tóm tắt paper/tài liệu cho task intern. | Mất rất nhiều não và sức lực; Workflow đọc tài liệu rất dễ dùng AI can thiệp. | Tài liệu chuyên ngành mới AI có hiểu đúng bối cảnh không? |
| 3 | Viết code tiền xử lý dữ liệu (data cleaning). | Việc này lặp đi lặp lại rất mỏi tay; AI sinh code cơ bản bây giờ làm rất tốt. | Format dữ liệu mỗi lúc một khác, lỡ AI sinh code bị lỗi thì mất công debug hơn tự viết. |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Soạn đề trắc nghiệm gia sư

```text
Problem 1 câu: Mất quá nhiều thời gian cuối tuần để tự chế và gõ các câu hỏi trắc nghiệm ôn tập cho học sinh dạy thêm.

Actor: Tuấn Tùng (Gia sư)

Thời điểm / bối cảnh: Tối thứ 7 hàng tuần, chuẩn bị tài liệu cho buổi dạy Chủ nhật.

Current workflow 3-7 bước:
1. Mở SGK xem tuần này học đến bài nào.
2. Lên Google tìm các đề trắc nghiệm cũ của bài đó.
3. Copy/paste câu hỏi ưng ý về file Word.
4. Tự chế lại số liệu hoặc đảo đáp án để tránh học sinh chép mạng.
5. Format lại file, lưu PDF và in ra.

Bottleneck: Bước 2 và Bước 4 (tìm mỏi mắt mới được câu hay, chế lại số liệu dễ bị sai hoặc mất thời gian giải thử lại).

Impact: Mất trắng 2 tiếng buổi tối cuối tuần đáng ra để đi chơi hoặc nghỉ ngơi.

Success metric: Rút ngắn thời gian ra đề từ 120 phút xuống còn 15-20 phút.

Non-AI alternative: Đi xin file đề của các anh chị gia sư khóa trước hoặc ra hiệu sách mua cuốn bài tập về photo.

AI hypothesis: Đưa tên bài học và độ khó vào prompt, AI sẽ tự động sinh ra 30 câu hỏi trắc nghiệm kèm đáp án và lời giải chi tiết.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
