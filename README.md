# Anti4

Trình duyệt anti-detect chạy hoàn toàn trên máy (offline-first) — quản lý nhiều hồ sơ trình duyệt với fingerprint, proxy, cookie, extension riêng biệt cho từng hồ sơ.

Repo này dùng để **phát hành bản cài đặt**. Mã nguồn không công khai ở đây.

## Tải về

👉 **[Tải bản mới nhất](https://github.com/anti4app/anti4/releases/latest)**

| | |
|---|---|
| Phiên bản | 1.0.0 |
| Hệ điều hành | macOS 10.13 trở lên |
| Chip | **Apple Silicon (M1/M2/M3/M4) — chưa hỗ trợ Mac chip Intel** |
| Dung lượng | ~10 MB |

## Cài đặt

1. Tải file `Anti4_1.0.0_aarch64.dmg`, mở ra và kéo **Anti4** vào thư mục **Applications**.

2. Bản này **chưa ký Apple Developer ID**, nên macOS sẽ chặn ở lần mở đầu tiên (báo *"Anti4 is damaged and can't be opened"* hoặc *"unidentified developer"*). Đây là cơ chế Gatekeeper của Apple với mọi app chưa ký, **không phải app bị lỗi hay nhiễm mã độc**.

   **Cách nhanh & chắc chắn nhất** — mở Terminal, dán lệnh sau rồi Enter:
   ```
   xattr -dr com.apple.quarantine /Applications/Anti4.app
   ```
   Sau đó mở Anti4 bình thường. Chỉ cần làm **một lần** sau mỗi lần cài/cập nhật.

   **Hoặc qua giao diện:**
   - **macOS 15 (Sequoia) trở lên:** mở Anti4 → hiện cảnh báo → bấm **Done** → vào  **System Settings → Privacy & Security**, kéo xuống thấy dòng *"Anti4 was blocked"* → bấm **Open Anyway**.
   - **macOS 14 trở xuống:** chuột phải vào **Anti4** → **Open** → bấm **Open** lần nữa.

   > Lưu ý: từ macOS 15, Apple đã **bỏ** cách chuột phải → Open, nên nếu dùng Sequoia anh/chị hãy làm theo lệnh Terminal hoặc đường System Settings ở trên.

## Cấu hình trình duyệt (bắt buộc)

Anti4 cần một bản **Chromium** để chạy hồ sơ. Bản cài này **không kèm sẵn** trình duyệt và tính năng tự động tải **chưa khả dụng** ở bản 1.0.0.

Sau khi mở app, nếu hiện thông báo tải trình duyệt thất bại, bấm **Continue anyway**, rồi vào **Settings** trỏ tới đường dẫn Chromium có sẵn trên máy.

> Để chống nhận diện (anti-detect) hoạt động đúng, nên dùng bản Chromium đã được vá — Chromium/Chrome tiêu chuẩn vẫn chạy được nhưng các tuỳ chỉnh fingerprint sẽ không có tác dụng đầy đủ.

## Bản quyền sử dụng

- Cài xong dùng **miễn phí 7 ngày**, không cần nhập key.
- Hết 7 ngày cần nhập **license key** để tiếp tục.
- Mỗi key kích hoạt cho **1 máy**, dùng **vĩnh viễn**.
- Sau khi kích hoạt, app **chạy được offline** — không cần kết nối mạng để kiểm tra bản quyền.

## Hỗ trợ

Gặp lỗi hoặc cần hỗ trợ: mở [Issue](https://github.com/anti4app/anti4/issues).
