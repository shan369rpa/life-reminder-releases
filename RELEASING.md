# Quy trình phát hành

Repo này không tự dựng gì cả. Bản cài được dựng trên máy rồi tải lên bằng tay —
dựng macOS đòi máy macOS, dựng Windows đòi chuỗi công cụ chéo, cả hai đều nằm ngoài
runner miễn phí của GitHub.

## 1. Chuẩn bị ở repo mã nguồn

```bash
# Đặt số phiên bản ở CẢ BA chỗ, phải khớp nhau
#   package.json           -> "version"
#   src-tauri/Cargo.toml   -> version
#   src-tauri/tauri.conf.json -> "version"

bunx tsc --noEmit && bun run build
hdiutil info | grep -i life-reminder   # còn volume .dmg cũ nào mount dở thì detach trước
bun run tauri:build
```

Bản cho cộng đồng bỏ nhánh Công cụ nội bộ:

```bash
VITE_PUBLIC_BUILD=1 bun run tauri:build
```

## 2. Kiểm trước khi tải lên

- [ ] Cài từ `.dmg` như một người dùng mới, không phải chạy từ thư mục build
- [ ] Thỉnh chuông ra đúng hai tiếng
- [ ] Nghe chuông chạy được, kéo được thanh tua
- [ ] Thêm một bài nhạc từ máy, tắt app mở lại vẫn còn
- [ ] Mở Cài đặt: cửa sổ riêng, chú tiểu vẫn đi lại được
- [ ] Đổi qua cả ba thứ tiếng
- [ ] Thoát bằng khay hệ thống, không còn tiến trình treo

## 3. Cập nhật nhật ký

Thêm một mục vào `CHANGELOG.md` theo mẫu **Thêm / Đổi / Sửa / Ghi chú**. Viết cho
người dùng đọc, không phải cho lập trình viên: nói cái gì đổi và họ sẽ thấy gì khác,
không nói tên hàm nào được sửa.

## 4. Tạo bản phát hành

```bash
VER=2.1.0
gh release create "v$VER" \
  --repo shan369rpa/life-reminder-releases \
  --title "v$VER" \
  --notes-file <(sed -n "/## \[$VER\]/,/^## \[/p" CHANGELOG.md | sed '$d') \
  "life-reminder_${VER}_aarch64.dmg" \
  "life-reminder_${VER}_x64-setup.exe"
```

Chưa có bản Windows thì bỏ file đó ra; trang web tự chuyển nút sang "Sắp có".

## 5. Cập nhật trang web

Sửa `VERSION` trong `web/src/config.ts` cho khớp, dựng lại rồi đăng.

## Quy ước đánh số

Theo [SemVer](https://semver.org/lang/vi/):

- **PATCH** (2.1.1) — chỉ sửa lỗi
- **MINOR** (2.2.0) — thêm chức năng, người dùng cũ không phải làm gì
- **MAJOR** (3.0.0) — đổi cách dùng hoặc đổi định dạng dữ liệu đã lưu

Tên thẻ luôn có tiền tố `v`: `v2.1.0`.
