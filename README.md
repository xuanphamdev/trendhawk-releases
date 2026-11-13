# TrendHawk – Radar Soi Kênh

Repo này **chỉ chứa bản cài đặt** và file quy tắc quét của TrendHawk. Không chứa mã nguồn.

## Tải về

Vào mục [Releases](https://github.com/xuanphamdev/trendhawk-releases/releases/latest) và chọn đúng file cho máy của bạn:

| Máy | File cần tải |
|---|---|
| Windows 10/11 | `TrendHawk-Setup-<phiên bản>.exe` |
| Mac chip Apple (M1, M2, M3, M4…) | `TrendHawk-<phiên bản>-arm64.dmg` |
| Mac chip Intel | `TrendHawk-<phiên bản>-x64.dmg` |

Máy cần có **Google Chrome**.

## Cảnh báo bảo mật khi cài lần đầu

TrendHawk chưa được ký số, nên máy sẽ hiện cảnh báo. Đây là điều bình thường.

**Windows:** khi thấy "Windows đã bảo vệ máy tính của bạn", bấm **Thông tin thêm**, rồi bấm **Vẫn chạy**.

**macOS:**
1. Mở file `.dmg`, kéo TrendHawk vào thư mục Applications.
2. Mở TrendHawk. Khi máy báo không mở được, bấm **Xong**.
3. Vào **Cài đặt hệ thống**, chọn **Quyền riêng tư & Bảo mật**, kéo xuống dưới và bấm **Vẫn mở**.

## File `rules.json`

Đây là quy tắc nhận dạng trang TikTok mà app tải về mỗi lần mở. File này chỉ chứa dữ liệu (selector, mẫu chữ, ngưỡng), không chứa mã chạy.

## Dữ liệu và quyền riêng tư

- Kết quả quét và lịch sử nằm **trên máy của bạn**, không gửi lên đâu cả.
  - Windows: `%APPDATA%\TrendHawk`
  - macOS: `~/Library/Application Support/TrendHawk`
- Khi quét, TrendHawk mở **một cửa sổ Chrome riêng** (hồ sơ riêng, không đăng nhập) và thu nhỏ xuống thanh tác vụ. Đừng đóng cửa sổ này khi đang quét; quét xong app tự đóng.
- Khi bạn bấm **phát clip**, link của clip đó được gửi tới dịch vụ bên ngoài **TikWM** hoặc **Tikmate** để lấy file video.
- Mỗi lần mở, app tải `rules.json` và kiểm tra bản mới trên trang Releases này. Hai việc này không gửi dữ liệu của bạn.

## Gỡ cài đặt

**Windows:** vào **Cài đặt → Ứng dụng**, chọn TrendHawk, bấm **Gỡ cài đặt**. Bộ gỡ sẽ hỏi có xóa luôn dữ liệu quét và lịch sử không.

**macOS:** kéo TrendHawk từ Applications vào Thùng rác. Dữ liệu vẫn còn ở `~/Library/Application Support/TrendHawk`; muốn xóa hẳn thì xóa thư mục này (Finder → Đi → Đi tới thư mục…).

**Bị phần mềm diệt virus chặn?** Vì app chưa được ký số, một số phần mềm diệt virus có thể chặn nhầm. Hãy ghi lại tên phần mềm và báo cho người hỗ trợ.
