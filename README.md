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
