# Anti4

Trình duyệt anti-detect chạy hoàn toàn trên máy (offline-first) — quản lý nhiều hồ sơ trình duyệt với fingerprint, proxy, cookie, extension riêng biệt cho từng hồ sơ.

Repo này dùng để **phát hành bản cài đặt**. Mã nguồn không công khai ở đây.

## Tải về

👉 **[Tải bản mới nhất](https://github.com/anti4app/anti4/releases/latest)**

| | |
|---|---|
| Phiên bản | 1.0.1 |
| Hệ điều hành | macOS 10.13 trở lên |
| Chip | **Apple Silicon (M1/M2/M3/M4) — chưa hỗ trợ Mac chip Intel** |
| Dung lượng | ~10 MB |

## Cài đặt

1. Tải file `Anti4_1.0.1_aarch64.dmg`, mở ra và kéo **Anti4** vào thư mục **Applications**.

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

## Trình duyệt — tự động tải lần đầu

Lần đầu mở app, Anti4 **tự tải trình duyệt stealth Chromium** (~145 MB) rồi cài vào thư mục dữ liệu của app. Quá trình này chỉ chạy **một lần**, có thanh tiến trình, và thường mất dưới một phút.

Trình duyệt được tải **trực tiếp từ bản phát hành chính chủ của [CloakBrowser](https://github.com/CloakHQ/CloakBrowser)** và được **đối chiếu SHA-256** trước khi cài — Anti4 không phân phối lại, không chỉnh sửa gì.

Nếu máy không có mạng hoặc bị chặn tải, bấm **Continue anyway** rồi vào **Settings** trỏ tay tới một bản Chromium có sẵn. (Lưu ý: Chrome/Chromium tiêu chuẩn vẫn chạy được nhưng các tuỳ chỉnh fingerprint sẽ không có tác dụng đầy đủ — nên dùng bản đã vá.)

## Bản quyền sử dụng

- Cài xong dùng **miễn phí 7 ngày**, không cần nhập key.
- Hết 7 ngày cần nhập **license key** để tiếp tục.
- Mỗi key kích hoạt cho **1 máy**, dùng **vĩnh viễn**.
- Sau khi kích hoạt, app **chạy được offline** — không cần kết nối mạng để kiểm tra bản quyền.

## Hỗ trợ

Gặp lỗi hoặc cần hỗ trợ: mở [Issue](https://github.com/anti4app/anti4/issues).
