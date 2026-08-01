# Nhật ký thay đổi

Định dạng theo [Keep a Changelog](https://keepachangelog.com/vi/1.1.0/); đánh số theo [Semantic Versioning](https://semver.org/lang/vi/).

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
