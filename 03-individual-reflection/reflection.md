# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Ngô Tuấn Tùng
- Mã học viên: 2A202602826
- Nhóm: Nhóm gồm 5 thành viên (Trần Văn Khánh, Ngô Tuấn Tùng, Cao Đức Hiệp, Đào Thị Huyền, Nguyễn Huy Cương)
- Candidate problem nhóm chọn: Tự động hóa việc đọc, trích xuất dữ liệu từ các tệp hóa đơn VAT (ảnh chụp/scan, PDF) và kiểm tra đối soát toán học để tự động điền vào file bảng kê chi phí Excel cho nhân viên kế toán nội bộ.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Scan 10 problems từ bối cảnh sinh viên năm 2 / Intern AI Engineer / gia sư; dùng 4 lăng kính (Lặp lại, Tốn thời gian, AI có thể tốt hơn, Pain từ người khác) | Đóng góp 3 candidates vào shortlist nhóm (#1 Debug code AI, #2 Đọc paper, #3 Chuẩn bị giáo án) |
| Pitch Problem Card | Pitch Problem Card #1 (Debug lỗi code AI): trình bày workflow 5 bước, bottleneck bước 3-4, metric giảm từ 30-90p xuống 20p | Nhóm hiểu rõ pain thật và đưa ra câu hỏi challenge về độ chính xác của AI khi chẩn đoán lỗi |
| Challenge bài của bạn khác | Đặt câu hỏi nghi vấn về bài hóa đơn Excel của Khánh: "Bài này dùng Rule/Regex đơn thuần được không, có thực sự cần AI không?" | Buộc cả nhóm phải làm rõ tỷ lệ hóa đơn ảnh chụp vs PDF điện tử, dẫn đến quyết định kiến trúc Workflow rõ ràng hơn |
| Gom trùng / cluster | Tham gia gom 12 candidates thành 4 cluster (A: Trích xuất dữ liệu văn phòng, B: Tổng hợp tri thức, C: Kỹ thuật chuyên sâu, D: Quản lý thời gian) | Xác định cluster A là nhóm khả thi cao nhất với workflow rõ, đo lường được |
| Chọn candidate problem | Bỏ phiếu và đồng thuận chọn bài hóa đơn kế toán (33/35 điểm) sau khi phân tích điểm mạnh/yếu của 3 shortlist candidates | Nhóm đạt đồng thuận nhanh, có ghi nhận disagreement và lý do chốt |
| Validation / research | Thực hiện phỏng vấn 2 kế toán viên; tham gia survey 12 người trên nhóm Zalo nghiệp vụ | Thu được quote thật (chị Mai, chị Lan) và tín hiệu phản bác về bảo mật dữ liệu, dẫn đến điều chỉnh boundary Human-in-the-loop |
| Workflow nhóm | Vẽ workflow hiện tại 6 bước và workflow tương lai 5 bước; xác định bottleneck bước 4 (gõ tay Excel chiếm 100/220 phút) | Before/after impact table rõ ràng: giảm 84% thời gian, 0% lỗi toán học lọt qua |
| Problem Statement | Đóng góp vào việc sửa v0→v1: bổ sung điều kiện ranh giới hóa đơn VAT tối đa 3 trang, tính toán metric dựa trên giả định tỷ lệ ảnh kém dưới 15% | PS v1 có metric cụ thể và boundary rõ hơn hẳn v0 |
| Rule / Workflow / Agent | Tham gia phân tích ma trận 3 mức: Rule (bất lực với ảnh chụp), Workflow (tối ưu), Agent (over-engineering) | Giúp nhóm hiểu tại sao Rule không đủ và Agent quá tốn kém, chốt Workflow là kiến trúc phù hợp |
| Decision | Tham gia thảo luận và đồng ý GO với pilot 30 hóa đơn, đo 3 số: thời gian, field accuracy, tỷ lệ chặn lỗi toán học | Decision GO được ghi chép đầy đủ với exit condition rõ ràng |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất là phần Disagreement trong Phase 3: tôi là người đặt câu hỏi "Bài hóa đơn dùng Rule/Regex thuần được không?" khiến nhóm phải phân tích sâu hơn tỷ lệ hóa đơn ảnh vs PDF, từ đó chốt ra kiến trúc Workflow kết hợp AI Vision + Rule Validation thay vì chỉ dùng Rule đơn thuần.
Tôi cũng đóng góp vào phần validation bằng cách trực tiếp phỏng vấn 2 kế toán viên và tổng hợp insight: nỗi đau không phải là tạo file Excel mà là căng thẳng khi đọc ảnh mờ và sợ gõ sai số tiền.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Hỏi AI gợi ý các problem tiềm năng từ bối cảnh sinh viên năm 2 / Intern AI Engineer / gia sư | Gợi ý được thêm các vấn đề về debug code, tìm tài liệu, chuẩn bị môi trường, ghi chú | AI đưa ra các ý quá lớn và mơ hồ như "AI giúp nghiên cứu AI tốt hơn" hoặc "xây agent tự làm project" mà không có workflow và số liệu cụ thể | Bỏ các ý không có actor + số đo cụ thể; chỉ giữ 10 problems có thời gian/tần suất đo được |
| Problem Card | Nhờ AI phản biện Problem Card #1 (Debug code AI) | AI chỉ ra bottleneck mô tả còn chung chung và thiếu metric về độ chính xác của đề xuất | AI phê bình quá rộng, không phân biệt các loại lỗi code cụ thể | Tự thu hẹp scope: chỉ áp dụng cho nhóm lỗi Python/PyTorch về matrix dimension và môi trường; bổ sung metric đếm số lần thử lại |
| Workflow | Không dùng | Không dùng — tự vẽ workflow 3 bước hiện tại và tương lai từ kinh nghiệm debug thực tế | — | — |
| Research | Dùng AI tra cứu nhanh các tool OCR/Document AI có sẵn trên thị trường | Liệt kê nhanh được ABBYY, AWS Textract, FPT.AI với mô tả tổng quan | AI mô tả tính năng theo quảng cáo, không chỉ ra khoảng trống phù hợp với bài toán hóa đơn Việt Nam | Tự vào link thực tế kiểm chứng; bổ sung góc nhìn "khoảng trống" và "bài học cho nhóm" dựa trên insight từ phỏng vấn kế toán |
| Problem Statement | Nhờ AI phản biện PS v0: hỏi field nào còn mơ hồ | AI chỉ ra metric "dưới 40 phút" chưa xét trường hợp ảnh mờ làm vỡ mốc; Boundary chưa nói rõ hóa đơn nhiều trang hoặc nước ngoài | AI chỉ phát hiện lỗi hiển nhiên, không gợi ý được con số ngưỡng cụ thể | Tự quyết định: giới hạn hóa đơn VAT Việt Nam tối đa 3 trang; metric tính trên giả định ảnh kém dưới 15% batch |
| Rule / Workflow / Agent | Dùng AI gợi ý ưu/nhược điểm của từng mức Rule/Workflow/Agent | Cung cấp được khung so sánh ban đầu về chi phí và độ phức tạp | AI gợi ý Agent theo kiểu lý thuyết sách vở, không bám vào thực tế là quy trình kế toán đi thẳng một chiều | Tự điền cột "Chọn?" dựa trên 5 câu hỏi chốt: loại Agent vì over-engineering, giữ Workflow vì bước cố định |
| Decision | Không dùng — tự chốt GO dựa trên 6 câu hỏi checklist từ worksheet | — | — | — |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Khi nghe top 3 problems của các bạn khác, điều tôi học được nhiều nhất là cách nhận ra sự khác biệt giữa một pain thật và một bất tiện có thể giải quyết bằng thói quen tốt hơn. Bài của Cương về theo dõi deadline hay bài của Hiệp về sắp xếp lịch cá nhân, tuy người thật có pain, nhưng khi nhóm đặt câu hỏi "Rule/template có giải được không?" thì câu trả lời là có, và đó là lúc tôi hiểu tại sao các bài đó không vào shortlist. Tôi cũng học được từ bài của Khánh (hóa đơn kế toán) rằng một bài toán đẹp không cần phức tạp, chỉ cần workflow rõ, số đo được và người chịu nỗi đau hiện diện ngay trong cuộc thảo luận.

Về phần tôi thay đổi ý kiến: lúc đầu tôi và Hiệp đặt câu hỏi nghi ngờ rằng bài hóa đơn có thể giải bằng Rule/Regex thuần và không nhất thiết cần AI. Sau khi Khánh và Huyền trình bày dữ liệu thực tế — hơn 30% hóa đơn là ảnh chụp từ điện thoại bị nghiêng, mờ hoặc không có text layer — tôi thực sự thay đổi quan điểm. Không phải vì áp lực, mà vì bằng chứng thuyết phục: Regex hoàn toàn bất lực trước ảnh chụp, và đó là điều không thể bỏ qua trong bài toán thực tế.

Điều khó nhất khi viết Problem Statement với tôi là phần Boundary, không phải Metric. Metric còn có thể đo bằng đồng hồ và tỷ lệ lỗi, nhưng Boundary đòi hỏi phải nghĩ ra tất cả những thứ hệ thống KHÔNG làm — và danh sách đó luôn bị bỏ sót những trường hợp biên. Ví dụ, ban đầu tôi không nghĩ đến hóa đơn nhiều trang hay hóa đơn nước ngoài cho đến khi AI phản biện v0, và ngay cả khi đó tôi phải tự quyết định ngưỡng "tối đa 3 trang" dựa trên thực tế, không phải AI gợi ý được.

Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm này: ngay từ Phase 3, tôi nên hỏi thẳng "Nếu không dùng AI mà chỉ cải tiến quy trình (process fix) thì giải được bao nhiêu % pain?" cho từng candidate, thay vì để câu hỏi đó xuất hiện muộn. Làm vậy sẽ loại nhanh hơn các bài thuộc Cluster D và tiết kiệm thời gian tranh luận.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

