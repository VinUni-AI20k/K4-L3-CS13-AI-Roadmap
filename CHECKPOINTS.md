# Các bước thực hành CS13

Mở file `[Nhom]_CS13.xlsx` đã lưu từ đúng đề. Các tên trang dưới đây là tên trong Excel. Tài liệu này giải thích cách làm; số liệu, điều kiện của từng sản phẩm nằm trong [hồ sơ tình huống](docs/CS13_HoSoTinhHuong.pdf).

## CP1 — Đọc cùng một hồ sơ, viết việc thành giả thuyết

- **Mục tiêu:** biết sản phẩm cần thay đổi điều gì cho người dùng và đo thay đổi đó thế nào.
- **Cần làm:** Nhiệm vụ 0 lúc 17:00–17:05; Nhiệm vụ 1 lúc 17:05–17:17. Điền `0_Đầu vào` và cột B–E của `1_Danh sách việc`.
- **Sản phẩm:** 6 mục đã đọc; ít nhất 5 việc có giả thuyết, chỉ số và ngưỡng.
- **Cần hiểu:** tên tính năng nói bạn xây gì; giả thuyết nói bạn kỳ vọng tạo ra kết quả nào và dùng số nào để kiểm chứng.
- **Tự kiểm tra:** `0_Đầu vào!B12` là 6; mỗi việc được giữ lại có đủ cột D–E, cột O không báo `Thiếu`.

### Viết gì để không chỉ liệt kê tính năng?

Mỗi đề định nghĩa riêng **“1 việc”**: một hóa đơn, một bài viết hoặc một bản nháp tóm tắt ra viện. Hãy dùng đúng đơn vị đó khi nói về hiệu quả và chi phí. Nếu lúc tính dùng một hóa đơn nhưng lúc đặt mục tiêu lại dùng một khách hàng, nhóm sẽ khó giải thích con số của mình.

Một **giả thuyết** là điều nhóm tin nhưng còn phải kiểm tra. Dùng khung: “Ta tin rằng làm [X] cho [Y] sẽ giúp đạt [Z]”. Sau đó, cột E phải cho biết nhìn vào chỉ số nào và bao nhiêu thì coi là đạt. “Nhanh hơn” chưa có ngưỡng; “giảm bao nhiêu phần trăm thời gian” là câu hỏi bạn cần trả lời. Những ngưỡng nhóm tự đề xuất cần được giải thích từ hồ sơ, không viết như kết quả đã đo được.

### Làm trong Excel

1. Cả nhóm đọc hồ sơ đúng đề. Ở `0_Đầu vào`, đánh dấu `Có` cho từng mục đã đọc, gồm cả kết quả đánh giá và giờ chuyên gia.
2. Chép 6 việc gợi ý của đề vào cột B–C của `1_Danh sách việc`. Nhóm được thêm việc; nếu bỏ hoặc đổi thứ tự, ghi lý do ở cột Q.
3. Viết giả thuyết ở cột D, chỉ số và ngưỡng bằng số ở cột E. Bảo đảm ít nhất 5 việc có nội dung đầy đủ.
4. Theo slide 81, hỏi công cụ AI sẵn có xem việc nào có thể được mô hình miễn phí làm thay trong 12 tháng. Đối chiếu gợi ý đó với hồ sơ để chuẩn bị chấm cột L ở CP2.

**Đọc checkpoint đúng cách:** cột O chỉ dò xem nội dung có chữ số hay không. Ô báo `Có` chưa chứng minh chỉ số hợp lý. Một người trong nhóm nên đọc thành tiếng một dòng: làm gì, giúp ai, đo bằng gì, bao nhiêu thì đạt. Nếu câu đó rõ, bạn đã có đầu vào để bàn về thứ tự ưu tiên.

## CP2 — Chấm điểm rồi quyết định tự làm, mua hay chờ

- **Mục tiêu:** chọn thứ tự công việc có căn cứ, thay vì chọn việc nghe hấp dẫn nhất.
- **Cần làm:** 17:17–17:30, điền cột F–L và P–Q của `1_Danh sách việc`.
- **Sản phẩm:** ít nhất 5 việc có điểm ở cột M và có quyết định ở cột P.
- **Cần hiểu:** điểm ưu tiên giúp so sánh; quyết định còn phải xét dữ liệu, khả năng đánh giá, công cụ có sẵn và điều kiện của đề.
- **Tự kiểm tra:** M–N đã hiện điểm, thứ hạng cho ít nhất 5 việc; giải thích được việc làm trước và các trường hợp đổi thứ tự.

### Các cột điểm có nghĩa gì?

**Độ phủ** là phạm vi người dùng hoặc công việc hưởng lợi; **tác động** là mức lợi ích; **mức tự tin** thể hiện bằng chứng nhóm đang có; **công sức** là lượng việc phải bỏ ra. File thực hành dùng thang rút gọn, khác một số thang trong lý thuyết RICE:

| Cột | Điền gì? | Giá trị |
|---|---|---|
| F, G, I | Độ phủ, tác động, công sức | 1–5; công sức không bằng 0 |
| H | Mức tự tin | 0,5 hoặc 0,8 hoặc 1 |
| J | Sẵn sàng dữ liệu | 0–1 |
| K | Sẵn sàng đánh giá | 0–1 |
| L | Rủi ro bị mô hình/nền tảng làm thay | 0–1 |

“Sẵn sàng đánh giá” hỏi liệu nhóm đã biết kiểm tra việc này đúng hay sai chưa. Có bộ đề 40 ca cho sản phẩm không có nghĩa mọi tính năng mới đều đã có bộ đề phù hợp. “Rủi ro bị nuốt” hỏi phần việc có dễ trở thành chức năng chung, sẵn có của mô hình hoặc phần mềm khác không. Điểm rủi ro càng cao thì hệ số độ bền càng thấp.

### Làm trong Excel

1. Chấm F–I cho từng việc, thống nhất cách hiểu thang điểm trong nhóm.
2. Dựa vào dữ liệu và kết quả đánh giá trong hồ sơ để chấm J–K; chấm L sau khi xem công cụ sẵn có và gợi ý AI đã đối chiếu.
3. Đọc điểm ở M và thứ hạng ở N. Hai cột này tự tính; không nhập đè công thức.
4. Ở P, chọn `Tự làm`, `Mua`, `Chờ` hoặc `Không làm`. Ở Q, ghi căn cứ khi mua, chờ, bỏ việc hoặc chọn thứ tự khác thứ hạng. Nếu chờ, xác định mốc xem lại trong lộ trình.

File tính điểm theo công thức sau; bạn chỉ cần hiểu các đầu vào, không tự viết lại trong ô xanh:

```text
RICE = Độ phủ × Tác động × Mức tự tin ÷ Công sức
Sẵn sàng trung bình = (Sẵn sàng dữ liệu + Sẵn sàng đánh giá) ÷ 2
Điểm AI = RICE × (0,5 + 0,5 × Sẵn sàng trung bình) × (1 − 0,5 × Rủi ro bị nuốt)
```

**Xong khi:** nhóm giải thích được vì sao việc chọn làm trước đáng làm trong điều kiện hiện có. Nhóm được chấm đầu vào khác bản mẫu; cần nhất quán và có căn cứ. Chuyển các việc đã chọn sang CP3 để quyết định AI được tự làm đến đâu.

## CP3 — Đặt cổng trước khi tăng mức tự động

- **Mục tiêu:** mô tả AI và người cùng làm việc thế nào, rồi đặt điều kiện để tăng quyền tự động.
- **Cần làm:** 17:30–17:43, điền `2_Mức tự động`.
- **Sản phẩm:** ít nhất 2 mức trong Mức 1–3 có cổng bằng số; có vai trò người duyệt, chi phí và biên lợi nhuận theo mức.
- **Cần hiểu:** đến ngày dự kiến chưa đủ để lên mức; phải qua cổng chất lượng và kiểm tra tính khả thi kinh tế.
- **Tự kiểm tra:** ít nhất 2 cổng có đủ chỉ số, ngưỡng, cỡ mẫu; ít nhất 1 mức có biên gộp từ 60% theo yêu cầu của file.

### “Cổng đánh giá” khác một lời hứa thế nào?

Cổng là điều kiện phải đo được trước khi cho AI tự làm nhiều hơn. “Đủ tốt thì triển khai” không cho người chấm biết kiểm tra bằng gì. Hãy ghi **chỉ số + ngưỡng + cỡ mẫu**, đồng thời làm rõ ai xác nhận. Nếu hồ sơ đã ghi một bản chưa được phát hành đầy đủ, cổng phải xử lý việc đó trước khi mở rộng.

Không quan sát thấy lỗi trên bộ đề nhỏ chưa đủ để kết luận tỷ lệ lỗi thực tế bằng 0. Slide 74 dùng quy tắc gần đúng `3/n`: khi thấy 0 lỗi trên n ca, giới hạn trên gần đúng của tỷ lệ lỗi ở mức tin cậy 95% là `3/n`. Đây là cách cân nhắc cỡ mẫu, không phải bảo đảm an toàn tuyệt đối.

### Làm trong Excel

1. Ở C–D, mô tả AI làm gì và người làm gì cho các mức cần thiết. Tên mức có sẵn ở B: Gợi ý, Hỗ trợ có duyệt, Tự động một phần, Tự động có giám sát.
2. Ở E, viết cổng cho ít nhất 2 mức trong Mức 1–3. Dùng kết luận đánh giá đúng đề; ghi chỉ số, ngưỡng, cỡ mẫu và người xác nhận. Mức 0 không được tính vào yêu cầu 2 cổng.
3. Điền điều kiện dữ liệu, hạ tầng, tuân thủ ở F và dự kiến nội bộ ở G. Ở H nhập tỷ lệ có dấu `%`, chẳng hạn `20%` thay vì `20`; ở I chọn người duyệt đúng đề.
4. Đọc chi phí J, biên gộp K và trạng thái L. Kiểm tra lại các đầu vào kinh tế B12–B20 trước khi dùng kết quả. Nếu sửa số liệu cho sẵn, phải có lý do của nhóm.

Chi phí người duyệt trong công thức chỉ tính **người của công ty cung cấp sản phẩm**. Riêng đề RaViện, bác sĩ bệnh viện luôn đọc, sửa và ký; dược sĩ của công ty là người được tính chi phí trong bảng. Đừng đổi vai trò để làm biên lợi nhuận đẹp hơn. Đề này cho phép ghi Mức 3 là `Không làm`.

**Xong khi:** nhóm có thể chỉ vào một mức và trả lời: AI làm gì, ai kiểm, phải vượt phép đo nào, trên bao nhiêu ca, với chi phí bao nhiêu. Nếu chưa đạt biên 60%, xem lại tỷ lệ duyệt của người công ty và giả định kinh tế; không hạ yêu cầu an toàn để đạt con số.

## CP4 — Ghép thành lộ trình và nộp bản trong lớp

- **Mục tiêu:** biến các quyết định vừa làm thành kế hoạch có điều kiện dừng và người xem lại.
- **Cần làm:** 17:43–17:55 điền trang 3–4; 17:55–18:00 kiểm tra trang 6, tải Excel lên repo nhóm và nộp link repo trên VLearn.
- **Sản phẩm:** tầng Bây giờ đủ 8 dòng, lịch rà soát, bản Excel có Nhiệm vụ 1–4.
- **Cần hiểu:** Bây giờ là cam kết gần; Tiếp theo là định hướng; Sau này là khám phá. Một lộ trình có thể được sửa khi bằng chứng thay đổi.
- **Tự kiểm tra:** `3_Bảng lộ trình!B5:B12` đủ 8 ô; trang 6 thường đạt 7/8, còn mục slide lãnh đạo làm ở nhà.

### Tám dòng của tầng Bây giờ lấy ở đâu?

| Dòng trong `3_Bảng lộ trình` | Lấy từ kết quả nào? |
|---|---|
| 5 · Việc chính | Các việc đã chọn ở trang 1 |
| 6 · Giả thuyết | Cột D trang 1 |
| 7 · Chỉ số và ngưỡng | Cột E trang 1 |
| 8 · Mức tự động | Trang 2 |
| 9 · Cổng đánh giá | Cổng phù hợp ở trang 2 |
| 10 · Điều kiện cần | Dữ liệu, hạ tầng, tuân thủ; khả năng huy động chuyên gia trong hồ sơ |
| 11 · Căn cứ kinh tế | Chi phí, biên gộp, biến nguy hiểm và kịch bản xấu của đề |
| 12 · Điều kiện dừng/đổi hướng | Một trạng thái đo được, thời điểm xem và hành động |

Điều kiện dừng viết theo khung: **NẾU [chỉ số chạm ngưỡng] VÀO [mốc xem xét] THÌ [dừng, đổi hướng hoặc lùi mức]**. Nếu điều kiện dùng tỷ lệ, cần biết đo trên quy mô nào. Kiểm tra quy mô thử nghiệm của đề có đủ để đo điều đó không; đừng lấy một chỉ số chỉ xuất hiện sau nhiều tháng để làm bằng chứng ngay ngày đầu.

### Làm trong Excel

1. Điền đủ B5:B12 của `3_Bảng lộ trình`. Cột B là Bây giờ 0–3 tháng; C là Tiếp theo 3–6 tháng; D là Sau này 6–12 tháng. C–D có thể hoàn thiện ở nhà nếu chưa kịp.
2. Ở `4_Rà soát`, điền chỉ số, quyết định có thể đưa ra và người quyết cho ngày 30/60/90. Điền cả các sự kiện có sẵn: mô hình/giá thay đổi, nền tảng/đối thủ có tính năng tương tự, quy định thay đổi.
3. Mở `6_Tự kiểm tra`. Sửa các mục còn `Xem lại`, trừ mục slide lãnh đạo sẽ làm ở CP5. Đọc lại nội dung dù ô đã báo `Đạt`: bộ kiểm tra chủ yếu đếm ô và dò chữ số.
4. Lưu, đóng rồi mở lại `[Nhom]_CS13.xlsx`. Tải file lên repo GitHub của nhóm; mỗi thành viên nộp link repo trên VLearn **trước 18:00 ngày 16/10/2026**. Xem thao tác tại [SUBMISSION.md](SUBMISSION.md).

**Xong khi:** đã có bản nộp mở được, đủ phần trong lớp và đúng đề. Đừng đợi làm slide rồi mới nộp lần đầu. Trang `5_Slide lãnh đạo` sẽ được bổ sung sau buổi học.

## CP5 — Làm một slide để lãnh đạo ra quyết định

- **Mục tiêu:** nói ngắn gọn nhóm đề nghị làm gì, cần gì và khi nào xem lại.
- **Cần làm:** ở nhà, hoàn thiện `5_Slide lãnh đạo` và tạo 1 slide; nộp trước 23:59 ngày 19/10/2026.
- **Sản phẩm:** 5 ô nội dung B4:B8 của trang 5 và một slide trình bày lộ trình.
- **Cần hiểu:** kết luận phải xuất hiện trước; số trên slide phải khớp lộ trình và tính toán trong Excel.
- **Tự kiểm tra:** D4:D8 đều `Đạt`; trang 6 đủ 8/8; slide có cùng kết luận, nguồn lực và mốc xem lại với Excel.

### Đưa gì lên slide?

Trang 5 có đúng 5 ô: **Kết luận**, **3 việc chính**, **Cần gì**, **Rủi ro lớn nhất & cách xử lý**, **Khi nào xem lại**. Mỗi ô không quá 60 chữ; cột C tự đếm và D báo trạng thái. Hãy điền bằng kết quả nhóm đã thống nhất, không bắt đầu một phương án khác ở phút cuối.

1. Điền B4:B8, đặt câu kết luận trước. Nguồn lực phải phù hợp với số giờ chuyên gia và điều kiện trong hồ sơ.
2. Sửa các ô báo `Trống` hoặc `Quá 60 chữ`; hoàn thiện phần Tiếp theo/Sau này nếu còn thiếu.
3. Chuyển nội dung thành **một slide** bằng công cụ trình chiếu sẵn có. Hồ sơ không bắt buộc một phần mềm hay phần mở rộng cụ thể cho slide.
4. Cập nhật bản Excel đã bổ sung trang 5 và thêm file slide vào cùng repo GitHub theo [SUBMISSION.md](SUBMISSION.md), trước **23:59 ngày 19/10/2026**.

**Xong khi:** bản Excel cuối đã có trang 5, slide đọc được và thông tin nộp trên VLearn đúng bài của nhóm. Điểm chính vẫn là thang sản phẩm 100 điểm; bản chuẩn của buổi học không có thuyết trình trên lớp.
