# Trạm Phước Đức — Ultra HD 2026

Website tĩnh được triển khai bằng GitHub Pages.

## Nội dung

- `index.html`: trang chủ Trạm Phước Đức.
- `.github/workflows/deploy.yml`: tự động triển khai lên GitHub Pages khi cập nhật nhánh `main`.

## Cách triển khai

1. Giải nén gói này.
2. Đưa `index.html`, `README.md` và thư mục `.github` lên thư mục gốc của repository GitHub.
3. Vào **Settings → Pages** và chọn **GitHub Actions** làm Build and deployment source.
4. Push thay đổi lên nhánh `main`. Workflow sẽ tự động triển khai website.
5. Mở tab **Actions** để xem trạng thái triển khai.

## Lưu ý

- File trang chủ phải giữ tên chính xác là `index.html`.
- Workflow cần quyền Pages và `id-token` đã khai báo trong file `deploy.yml`.
- Đồng hồ 100 năm lưu thời điểm bắt đầu trong `localStorage` của trình duyệt đang sử dụng; xóa dữ liệu trình duyệt có thể làm mốc bắt đầu được thiết lập lại.
