# CS13 — Lộ trình sản phẩm AI · Nhóm H3201 · Đề 1 SổSạch

**AI in Action · Track 1 · Khóa 4 · Level 3 · Thực hành chiều 16/10/2026**

Bài nhóm sau 3 giờ lý thuyết CS13. Câu hỏi của buổi: **làm việc gì trước, khi nào cho máy tự làm nhiều hơn, và khi nào thì dừng?** Lộ trình viết theo giả thuyết: *"Ta tin rằng làm X sẽ giúp Y đạt Z; biết đúng khi chỉ số W đạt ngưỡng V."*

- **Tên nhóm:** H3201
- **Đề:** 1 · SổSạch — đọc hoá đơn đầu vào (làm từ [`src/CS13_Roadmap_De1.xlsx`](src/CS13_Roadmap_De1.xlsx))
- **Thành viên và đóng góp:** [team/TEAM.md](team/TEAM.md)
- **Báo cáo nhóm:** [report/team/group_report.md](report/team/group_report.md)

## Bài làm

| File | Là gì |
|---|---|
| [`H3201_CS13.xlsx`](H3201_CS13.xlsx) | **Bài nộp chính** — Excel đã điền Nhiệm vụ 0–5, tự kiểm tra 8/8 |
| [`H3201_CS13_Slide.pptx`](H3201_CS13_Slide.pptx) | 1 slide lãnh đạo (CP5), dựng từ 5 ô của trang `5_Slide lãnh đạo` |
| [`H3201_CS13_Slide.pdf`](H3201_CS13_Slide.pdf) | Cùng slide, bản PDF để xem nhanh trên GitHub |

## Thành viên nhóm H3201

| STT | Họ và tên | MSSV |
|---|---|---|
| 1 | Phan Duy Thành | 2A202602930 |
| 2 | Chử Trần Phương Nam | 2A202602675 |
| 3 | Phùng Gia Khánh | 2A202602585 |
| 4 | Bùi Hải Nam | 2A202602636 |
| 5 | Tô Anh Đức | 2A202602639 |

## Đề của nhóm

> **Đề 1 — SổSạch:** trợ lý đọc hoá đơn đầu vào cho văn phòng kế toán dịch vụ.
> **1 việc** = 1 hoá đơn được đọc, đối chiếu và nhập vào phần mềm kế toán.
> Văn phòng thử nghiệm phụ trách 40 doanh nghiệp, khoảng 12.000 hoá đơn/tháng. Bản 2 (đọc ảnh hai bước, rẻ hơn 20%) đã qua cổng phát hành: 97,3% ≥ 95%, 0 lỗi nghiêm trọng, kappa 0,90.
> Chuyên gia: chị Hạnh (kế toán trưởng, 3 giờ/tuần) và anh Tùng (trưởng nhóm nhập liệu).
> *"Sai mã số thuế hay sai tiền thì không được lần nào."* (chị Hạnh)

Mọi số kinh tế lấy đúng từ hồ sơ tình huống (trang `2_Mức tự động`, dòng 12–20).

## Đã làm gì

| Trang | Nội dung |
|---|---|
| `0_Đầu vào` | Đánh dấu đã đọc 6/6 mục, ghi chú số liệu chính của đề |
| `1_Danh sách việc` | 7 việc (6 việc gợi ý + 1 việc nhóm thêm), mỗi việc có giả thuyết, chỉ số có con số, điểm ưu tiên, quyết định và lý do |
| `2_Mức tự động` | 4 mức, mức 1–3 có cổng đánh giá (chỉ số + ngưỡng + cỡ mẫu), vai trò người duyệt, chi phí và biên lợi nhuận theo mức |
| `3_Bảng lộ trình` | Bây giờ (0–3 tháng) / Tiếp theo (3–6 tháng) / Sau này (6–12 tháng), đủ 8 dòng mỗi tầng |
| `4_Rà soát` | Mốc ngày 30/60/90 và 3 sự kiện (mô hình mới, đối thủ, pháp lý) |
| `5_Slide lãnh đạo` | 5 ô, mỗi ô 40–57 chữ (giới hạn 60) → chuyển thành [1 slide](H3201_CS13_Slide.pdf) |
| `6_Tự kiểm tra` | 8/8 Đạt |

### Thứ tự ưu tiên

Điểm = Độ phủ × Tác động × Mức tự tin ÷ Công sức × (0,5 + 0,5 × sẵn sàng trung bình) × (1 − 0,5 × rủi ro bị nuốt)

| Hạng | Việc | Điểm | Quyết định | Vì sao |
|---|---|---|---|---|
| 1 | Đối chiếu mã số thuế người bán | 15,00 | Mua | Dịch vụ tra cứu có sẵn, chấm 100% bằng mã lệnh, trúng điều "sai mã số thuế không được lần nào" |
| 2 | Gắn cờ hoá đơn cần người xem | 7,88 | Tự làm | Quyết định % người duyệt, tức chi phí mỗi hoá đơn |
| 3 | Kiểm tra số tiền và hoá đơn trùng *(nhóm thêm)* | 6,63 | Tự làm | Mã lệnh, rẻ, trúng điều "sai tiền không được lần nào" |
| 4 | Nhập tự động hoá đơn điện tử | 4,88 | Mua | Phần mềm kế toán đã có sẵn tính năng, chỉ cần nối |
| 5 | Đọc ảnh hoá đơn giấy | 3,77 | Tự làm | Bản 2 đã có, chỉ phủ phần hoá đơn ảnh |
| 6 | Gợi ý tài khoản hạch toán | 1,20 | Chờ | Chưa có dữ liệu hạch toán của khách hàng |
| 7 | Trả lời câu hỏi thuế chung | 0,23 | Không làm | Ngoài "1 việc", rủi ro pháp lý, dễ bị chatbot chung nuốt |

### Mức tự động và kinh tế

Chi phí mỗi hoá đơn = 254 đ (gọi AI) + 200 đ (hạ tầng) + % duyệt × 1,5 phút × 50.000 đ/giờ. Doanh thu 3,97 triệu/văn phòng, 1.760 hoá đơn/văn phòng/tháng.

| Mức | % người duyệt | Chi phí/hoá đơn | Biên gộp | Cổng để lên mức | Dự kiến |
|---|---|---|---|---|---|
| 0 · Gợi ý | 100% | 1.704 đ | 24,5% | Không cần (bản 2 đã qua cổng phát hành) | Tuần 1–2 |
| 1 · Hỗ trợ có duyệt | 20% | 704 đ | 68,8% | ≥ 500 hoá đơn chạy song song 2 tuần, 0 lỗi mã số thuế/tiền ngoài cờ, cờ ≤ 20% | Tháng 1 |
| 2 · Tự động một phần | 10% | 579 đ | 74,3% | ≥ 8 tuần ở Mức 1, ≥ 3.000 hoá đơn: 0 lỗi lọt, đạt ≥ 98%, cờ thừa ≤ 30%, ≥ 10 văn phòng | Tháng 4–5 |
| 3 · Tự động có giám sát | 5% | ~517 đ | 77,1% | ≥ 3 tháng ở Mức 2, ≥ 20.000 hoá đơn điện tử: 0 lỗi nghiêm trọng, đạt ≥ 99,5% (chỉ tầng Thường) | Tháng 9–12 |

Mức 0 lỗ biên (24,5%) nên phải lên Mức 1 ngay trong tháng 1.

### Điều kiện dừng

- **Bây giờ:** 1 lỗi mã số thuế hoặc tiền lọt vào sổ → hạ ngay về Mức 0; tỷ lệ cờ > 30% hai tuần liên tiếp → dừng ở Mức 0, sửa cờ. Điều kiện này đo được ngay trên ~12.000 hoá đơn/tháng của văn phòng thử nghiệm.
- **Tiếp theo (theo đề):** NẾU doanh thu bình quân dưới 3,71 triệu/văn phòng trong 2 tháng liên tiếp, trên ít nhất 10 văn phòng, THÌ dừng mở rộng.
- **Rủi ro lớn nhất:** doanh thu bình quân (65% doanh thu đến từ 30% văn phòng dùng nhiều), kịch bản xấu hết tiền ở tháng 7.

## Giả định của nhóm (không có trong đề)

- Phần lớn hoá đơn đầu vào đã là hoá đơn điện tử, nên việc đọc ảnh chỉ phủ một phần (độ phủ 3/5).
- Các cỡ mẫu 500 / 3.000 / 20.000 hoá đơn, mốc thời gian lên Mức 2 và Mức 3, % duyệt ở Mức 3 (5%).
- Phần tuân thủ dẫn Luật Trí tuệ nhân tạo số 134/2025/QH15 ở mức chung; đề dặn đọc văn bản gốc trước khi ghi vào bài, nhóm chưa đối chiếu chi tiết.

## Tài liệu đề bài (giữ nguyên từ repo đề)

| File | Nội dung |
|---|---|
| [RULES.md](RULES.md) | Luật làm bài |
| [CHECKPOINTS.md](CHECKPOINTS.md) | Các bước CP1 → CP5 |
| [RUBRIC.md](RUBRIC.md) | Thang chấm 100 điểm |
| [SUBMISSION.md](SUBMISSION.md) | Hai hạn nộp và checklist |
| [docs/](docs/README.md) | Hồ sơ tình huống và slide bài giảng gốc |
| [src/](src/README.md) | File Excel đề gốc (Đề 1–3) và bản mẫu |
