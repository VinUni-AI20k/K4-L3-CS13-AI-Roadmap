---
title: "CS13 — Lộ trình sản phẩm AI"
description: "Làm theo nhóm: lập lộ trình 12 tháng trên Excel và tóm tắt thành một slide."
requiredTools:
  - "Excel hoặc LibreOffice"
requiresSubmission: true
workMode: "team"
---

# CS13 — Lộ trình sản phẩm AI

**Track 1 · Khóa 4 · 60 phút thực hành ngày 16/10/2026.**

Nhóm bạn sẽ quyết định: **làm gì trước, khi nào tăng mức tự động, khi nào dừng**. Bài nộp là một file Excel; slide lãnh đạo làm ở nhà. Không cần viết code hoặc API key.

Tài liệu: [K4-L3-CS13-AI-Roadmap](https://github.com/VinUni-AI20k/K4-L3-CS13-AI-Roadmap) — repo private, cần tài khoản được cấp quyền.

## 1. Mở đúng đề — 5 phút

1. Theo số nhóm, tải file Excel tương ứng và hồ sơ tình huống trong bộ tài liệu CS13.
2. Lưu bản làm bài thành `[Nhom]_CS13.xlsx`. Chỉ điền ô vàng; ô xanh tự tính.
3. Đọc hồ sơ đúng đề, đánh dấu 6 mục đã đọc trong trang `0_Đầu vào`.

| Số nhóm | Đề | File trong thư mục `src/` |
|---|---|---|
| 1, 4, 7, 10… | SổSạch — đọc hóa đơn | `CS13_Roadmap_De1.xlsx` |
| 2, 5, 8, 11… | ChấmNhanh — chấm bài viết | `CS13_Roadmap_De2.xlsx` |
| 3, 6, 9, 12… | RaViện — soạn nháp tóm tắt ra viện | `CS13_Roadmap_De3.xlsx` |

Hồ sơ nằm ở `docs/CS13_HoSoTinhHuong.pdf`. Số liệu kinh tế đã có ở trang `2_Mức tự động`, dòng 12–20. Có thể xem `CS13_Roadmap_Mau.xlsx` để hiểu cách điền; mẫu là sản phẩm khác, không chép số.

**Xong khi:** trang `0_Đầu vào` ghi đủ 6/6 mục, cả nhóm biết “1 việc” trong đề là gì.

## 2. Viết ít nhất 5 giả thuyết — 12 phút

Một tên tính năng chưa nói được lợi ích. Giả thuyết cần cho biết **làm gì → giúp ai → đạt kết quả nào**, rồi có số để kiểm chứng.

1. Mở `1_Danh sách việc`, chép 6 việc gợi ý của đề vào cột B–C.
2. Ở D, viết: “Ta tin rằng làm [X] cho [Y] sẽ đạt [Z]”.
3. Ở E, ghi chỉ số và ngưỡng bằng số. Tránh chỉ ghi “nhanh hơn”, “chính xác hơn”.
4. Hỏi AI xem việc nào dễ được mô hình miễn phí làm thay; đối chiếu gợi ý với hồ sơ để dùng ở bước 3.

**Xong khi:** ít nhất 5 việc có đủ D–E, cột O không báo `Thiếu`. Nhóm giải thích được con số mình chọn; ô `Có` chỉ cho biết file đã tìm thấy chữ số.

## 3. Chấm điểm và chọn việc làm trước — 13 phút

Vẫn ở `1_Danh sách việc`, điền các đầu vào sau:

| Cột | Nội dung | Thang điểm |
|---|---|---|
| F, G, I | Độ phủ, tác động, công sức | 1–5 |
| H | Mức tự tin | 0,5 / 0,8 / 1 |
| J, K | Sẵn sàng dữ liệu, sẵn sàng đánh giá | 0–1 |
| L | Rủi ro bị mô hình/nền tảng làm thay | 0–1 |

1. Chấm F–L dựa trên hồ sơ. Có bộ đề cho sản phẩm không có nghĩa mọi việc mới đều đã đánh giá được.
2. Đọc điểm và thứ hạng tự tính ở M–N; không sửa công thức.
3. Ở P chọn `Tự làm`, `Mua`, `Chờ` hoặc `Không làm`. Ghi căn cứ ở Q, nhất là khi bỏ việc hoặc đổi thứ tự.

Điểm = Độ phủ × Tác động × Tự tin ÷ Công sức × (0,5 + 0,5 × Sẵn sàng trung bình) × (1 − 0,5 × Rủi ro bị nuốt).

**Xong khi:** ít nhất 5 việc có điểm; nhóm giải thích được vì sao chọn việc đầu tiên. Điểm giúp so sánh, không thay nhóm ra quyết định.

## 4. Đặt cổng trước khi tăng tự động — 13 phút

**Cổng đánh giá** là điều kiện phải vượt trước khi lên mức tự động: **chỉ số + ngưỡng + cỡ mẫu**. Đến ngày dự kiến chưa đủ để lên mức.

1. Mở `2_Mức tự động`. Điền AI làm gì ở C, người làm gì ở D.
2. Ở E, đặt cổng cho ít nhất 2 mức trong Mức 1–3; làm rõ ai xác nhận. Ghi điều kiện dữ liệu, hạ tầng, tuân thủ ở F và dự kiến ở G.
3. Điền tỷ lệ duyệt ở H bằng dạng `%`, chọn đúng người duyệt ở I. Đọc chi phí J, biên gộp K; yêu cầu file là ít nhất 1 mức có biên từ 60%.
4. Kiểm tra cổng có xử lý kết luận đánh giá hiện tại của đề chưa: ChấmNhanh chỉ phát hành có giới hạn; RaViện chưa phát hành.

**Riêng RaViện:** bác sĩ bệnh viện luôn đọc, sửa và ký; chi phí người duyệt của công ty là dược sĩ. Mức 3 có thể ghi `Không làm`. Không bỏ bước an toàn để làm đẹp biên lợi nhuận.

**Xong khi:** có 2 cổng đủ chỉ số, ngưỡng, cỡ mẫu; rõ vai trò người duyệt và chi phí. Có thể xem quy tắc gần đúng `3/n` ở slide 74 khi cân nhắc cỡ mẫu: 0 lỗi quan sát không chứng minh tỷ lệ lỗi thực bằng 0.

## 5. Điền lộ trình, kiểm tra và nộp — 17 phút

Trong `3_Bảng lộ trình`, Bây giờ là 0–3 tháng, Tiếp theo 3–6 tháng, Sau này 6–12 tháng. Ưu tiên làm đủ tầng Bây giờ trong lớp.

1. Điền B5:B12, đủ 8 dòng: việc chính; giả thuyết; chỉ số/ngưỡng; mức tự động; cổng; điều kiện cần; căn cứ kinh tế; điều kiện dừng.
2. Viết điều kiện dừng: **NẾU [chỉ số chạm ngưỡng] VÀO [mốc xem xét] THÌ [dừng/đổi hướng/lùi mức]**. Dùng quy mô đo phù hợp với đề.
3. Trong `4_Rà soát`, điền chỉ số, quyết định và người quyết cho ngày 30/60/90 cùng các sự kiện có sẵn.
4. Mở `6_Tự kiểm tra`, sửa mục còn thiếu. Lưu và nộp `[Nhom]_CS13.xlsx` lên VLearn **trước 18:00 ngày 16/10/2026**.

**Xong khi:** tầng Bây giờ đủ 8 ô, đã có lịch rà soát và file nộp mở được. Bản trong lớp thường đạt 7/8 mục vì slide lãnh đạo làm ở nhà. Tiếp theo/Sau này có thể hoàn thiện ở nhà nếu chưa kịp.

## 6. Ở nhà: làm một slide lãnh đạo

1. Điền B4:B8 của `5_Slide lãnh đạo`: kết luận; 3 việc chính; cần gì; rủi ro/cách xử lý; khi nào xem lại.
2. Mỗi ô không quá 60 chữ; sửa đến khi D4:D8 đều `Đạt`. Chuyển nội dung thành **1 slide**.
3. Nộp Excel đã bổ sung và slide lên mục VLearn do lớp cung cấp, **trước 23:59 ngày 19/10/2026**, giờ Việt Nam.

**Xong khi:** trang 6 đạt 8/8; slide khớp số liệu và quyết định trong Excel. Bản chuẩn không có thuyết trình trên lớp.

Điểm chính: **giả thuyết 20 · ưu tiên 20 · mức tự động/cổng 25 · điều kiện/rủi ro 15 · slide 20**. Giảng viên chấm nội dung; ô `Đạt` không tự quy đổi thành điểm. Bài muộn vẫn nhận, giảng viên quyết định việc trừ điểm.
