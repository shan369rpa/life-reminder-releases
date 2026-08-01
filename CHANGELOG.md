# Nhật ký thay đổi

Định dạng theo [Keep a Changelog](https://keepachangelog.com/vi/1.1.0/); đánh số theo [Semantic Versioning](https://semver.org/lang/vi/).

## [2.2.1] — 2026-08-01

### Sửa

- **Sửa vị trí nút dừng nhạc.** Di chuyển nút dừng nhạc nổi từ góc trên phải xuống gần nhân vật để tránh bị lém/cắt trên màn hình có tai thỏ (notch) hoặc do safe area inset của macOS.

## [2.2.0] — 2026-08-01

### Thêm

- **Nghe nhạc thì nhắm mắt.** Bật một bài thiền ca, Breath Chime nhắm mắt lại lắng nghe cùng bạn — không chắp tay, chỉ ngồi yên. Riêng bài chuông vẫn chắp tay chào, đó là nghi thức.
- **Nút dừng nhạc nổi.** Đóng bảng Thiền ca mà nhạc còn chạy thì một nút dừng nhỏ hiện ở góc trên phải màn hình. Trước đây muốn dừng phải mở lại bảng.
- **Bài chuông bảy phút vào luôn danh sách Thiền ca** — thành năm bài đóng kèm. Phát từ nhánh Chuông hay từ bảng đều là một bài, bấm dừng ở đâu cũng dừng.

### Đổi

- **Hành vi gọn lại còn hai chế độ.** Trước đây có hai núm chồng lấn nhau — "Mức năng động" ba bậc và ô tích "Tự làm việc riêng", tổng cộng sáu tổ hợp. Giờ chỉ còn: **Tĩnh** (ngồi yên một chỗ, thi thoảng nhắm mắt thiền, không bao giờ tự dịch chuyển) hoặc **Tự làm việc riêng**. Cài đặt cũ của bạn được chuyển sang tương đương, không phải chỉnh lại.
- **Ngồi thiền giờ chỉ nhắm mắt, không chắp tay.** Chắp tay là cử chỉ chào, không phải tư thế ngồi.

### Bỏ

- **Tự đi theo con trỏ chuột.** Một nhân vật thiền bám theo con trỏ đọc ra như đang đòi được chú ý. Mắt vẫn dõi theo chuột như cũ — chỉ bỏ việc đi theo.
- Hai nhánh **Ngồi thiền** và **Đi thiền** tạm rút khỏi vòng kỹ năng: chế độ Tĩnh đã lo phần ngồi thiền, còn đi thiền chờ có tư thế đứng mới ra dáng đi thật.

### Sửa

- **Bấm vào khoảng trống quanh Breath Chime giờ xuyên xuống ứng dụng bên dưới.** Cửa sổ rộng hơn nhân vật khá nhiều, mà phần trong suốt vẫn nuốt chuột — bấm vào đó là ứng dụng phía sau không nhận được gì.
- **Ctrl+A trong bảng không còn bôi đen cả bảng**, chỉ ô nhập liệu mới chọn được chữ.
- **Kéo thanh trượt trong Cài đặt không còn giật.**

### Ghi chú

- Bản cài chưa được ký số. Xem [README](README.md#cài-đặt) để biết cách mở lần đầu.
- Bản macOS dành cho Apple Silicon (M1 trở lên).

## [2.1.0] — 2026-08-01

### Thêm

- **Nhánh Chuông tách làm hai đường.** *Thỉnh chuông* đánh hai nhịp ngân chồng lên nhau như chuông thật. *Nghe chuông* phát trọn bài chuông bảy phút, bấm lại để dừng.
- **Thiền ca.** Bốn bài đóng kèm ngay trong ứng dụng, không cần mạng. Thêm nhạc riêng thì chọn file từ máy — ứng dụng chép vào kho của nó, tắt máy mở lại vẫn còn.
- **Đi thiền.** Chú tiểu đi chậm qua lại trên màn hình, mỗi lần quay đầu thì dừng lại cúi chào. Vừa là một nhánh kỹ năng, vừa thi thoảng tự làm.
- **Hành vi tự phát.** Chú tiểu tự ngồi, tụng kệ, ngó nghiêng, dạo một quãng. Tắt được trong Cài đặt.
- **Ba thứ tiếng** — Việt · English · Français. Đổi một lần là đổi hết, kể cả câu kệ.
- **Thanh chỉnh tốc độ đi** trong Cài đặt (40–320 px/giây).
- **Bảng Cài đặt gập được từng mục**: Chuông · Giờ yên lặng · Hình dáng · Hành vi · Âm thanh · Ngôn ngữ.

### Đổi

- **Các bảng chuyển sang cửa sổ riêng.** Trước đây bảng nằm chung cửa sổ với chú tiểu nên chú tiểu phải đứng yên suốt thời gian bảng mở. Giờ hai cửa sổ độc lập: mở Cài đặt mà chú tiểu vẫn đi lại được, và bảng đứng yên tại chỗ khi chú tiểu di chuyển.
- **Cài đặt tự lưu.** Bỏ hẳn nút Lưu. Sửa tới đâu ghi tới đó, kèm dòng "✓ Đã lưu HH:MM:SS" và ô vừa đổi nháy viền xanh.
- **Nhạc phát qua giao thức asset://** nên kéo được thanh tua và không phải nạp cả bài vào bộ nhớ.
- **Vòng kỹ năng gọn lại còn sáu nhánh**, những việc không thuộc thực tập chánh niệm lùi vào nhánh *Khác*.
- Con số cạnh thanh trượt trong Cài đặt đổi ngay trong lúc kéo.

### Sửa

- Đổi kích thước chú tiểu làm mất hết cử động (thở, chớp mắt, lắc thân). Nguyên nhân: mỗi hoạt cảnh CSS chạm tới `transform` đều nuốt mất tỉ lệ phóng.
- Chú tiểu đông cứng giữa một khung hình khi cửa sổ bị một ứng dụng toàn màn hình che.
- Thỉnh chuông nhiều nhịp thì nhịp sau cắt cụt nhịp trước.
- Chú tiểu có thể đi ra ngoài mép màn hình.

### Ghi chú

- Bản cài chưa được ký số. Xem [README](README.md#cài-đặt) để biết cách mở lần đầu.
- Bản macOS dành cho Apple Silicon (M1 trở lên).

[2.1.0]: https://github.com/shan369rpa/life-reminder-releases/releases/tag/v2.1.0
[2.2.0]: https://github.com/shan369rpa/life-reminder-releases/releases/tag/v2.2.0
