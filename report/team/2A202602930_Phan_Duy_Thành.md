# Báo cáo cá nhân — Phan Duy Thành

## 1. Thông tin thành viên

- Họ tên: Phan Duy Thành
- MSSV: 2A202602930
- Nhóm và đề CS13: Nhóm H3201 · Đề 1 — SổSạch (trợ lý đọc hoá đơn đầu vào)

## 2. Phần việc phụ trách

- Trưởng nhóm, giữ file [`H3201_CS13.xlsx`](../../H3201_CS13.xlsx) và chia sẻ màn hình để cả nhóm cùng quyết định.
- **CP4 · Bảng lộ trình và lịch rà soát:** trang `3_Bảng lộ trình` và `4_Rà soát`.
- Tạo repo GitHub, tải bài lên và kiểm tra trang `6_Tự kiểm tra` trước khi nộp.

## 3. Đóng góp cụ thể

- Ghép kết quả CP1–CP3 thành lộ trình 3 tầng **Bây giờ (0–3 tháng) / Tiếp theo (3–6 tháng) / Sau này (6–12 tháng)**, đủ 8 dòng mỗi tầng:
  - Bây giờ: làm trước đối chiếu mã số thuế (Mua), kiểm tra tiền và hoá đơn trùng, gắn cờ; chạy bản 2 ở Mức 1 (kế toán viên duyệt 20%, 704 đ/hoá đơn, biên 68,8%).
  - Tiếp theo: thu hẹp cờ để lên Mức 2 (duyệt 10%, biên 74,3%), mở rộng lên 10–20 văn phòng.
  - Sau này: Mức 3 chỉ cho hoá đơn điện tử tầng Thường; thử gợi ý tài khoản hạch toán ở Mức 0.
- Viết điều kiện dừng đo được ngay trên quy mô thử nghiệm (~12.000 hoá đơn/tháng): **1 lỗi mã số thuế hoặc tiền lọt vào sổ → hạ ngay về Mức 0; tỷ lệ cờ > 30% hai tuần liên tiếp → dừng ở Mức 0, sửa cờ.** Điều kiện của đề về doanh thu bình quân (< 3,71 triệu/văn phòng 2 tháng liên tiếp trên ≥ 10 văn phòng) để ở tầng Tiếp theo vì cần nhiều văn phòng và nhiều tháng mới đo được.
- Lập lịch rà soát ngày 30/60/90 (chỉ số cần nhìn, quyết định đi tiếp/sửa/đổi hướng/dừng, người quyết) và 3 sự kiện kích hoạt: mô hình mới hoặc giá gọi AI giảm, nền tảng/đối thủ ra tính năng tương tự, quy định pháp lý thay đổi.
- Tạo repo, tải Excel và slide lên, soát trang `6_Tự kiểm tra` đạt 8/8.

## 4. Bằng chứng

- `3_Bảng lộ trình!B5:D12` — 3 tầng lộ trình, gồm điều kiện dừng ở dòng 12.
- `4_Rà soát!B5:D10` — mốc 30/60/90 và 3 sự kiện.
- `6_Tự kiểm tra!C5:C12` — 8/8 Đạt.
- Repo nhóm: https://github.com/thanhpd123/Track01_Day28_3201

## 5. Tự đánh giá

- **Điều hiểu rõ:** đến ngày dự kiến chưa đủ để tăng mức tự động; phải qua cổng có chỉ số + ngưỡng + cỡ mẫu. Điều kiện dừng phải đo được ở đúng quy mô đang có — nên tầng Bây giờ dùng lỗi lọt và tỷ lệ cờ (đo hằng tuần trên ~12.000 hoá đơn), còn doanh thu bình quân chỉ có ý nghĩa khi đã có ≥ 10 văn phòng.
- **Giả định còn cần kiểm chứng:** nhóm giả định phần lớn hoá đơn đầu vào đã là hoá đơn điện tử, nên việc đọc ảnh chỉ phủ một phần. Cần đo tỷ lệ hoá đơn ảnh thật ở mốc ngày 30; nếu tỷ lệ này cao hơn dự kiến thì phải xem lại thứ tự ưu tiên và lịch lên Mức 3.
