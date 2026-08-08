# 🌟 Trạm Phước Đức - Modern Spiritual Hub

> **Trạm Phước Đức** là ứng dụng web cá nhân mang phong cách hiện đại (Modern Spiritual), được thiết kế tối ưu cho nền tảng di động và máy tính bảng. Ứng dụng tích hợp hệ thống đếm niệm lành hằng ngày, widget lịch, danh ngôn tâm linh ngẫu nhiên cùng hệ sinh thái các liên kết tu tập và tra cứu.

---

## 🚀 Tính Năng Nổi Bật

*   🕒 **Widget Ngày & Trạng Thái:** Tự động cập nhật ngày tháng theo chuẩn Việt Nam và hiển thị trạng thái ngày chay / ngày thường dựa theo lịch dương/âm.
*   🙏 **Bộ Đếm Niệm Lành (Gieo Duyên):** Cho phép người dùng tương tác để niệm Phật/niệm câu lành, tự động lưu trữ số liệu cá nhân qua `localStorage`.
*   📜 **Lời Khuyên Tâm Linh:** Cung cấp các câu nói, triết lý sống thiện lành ngẫu nhiên với nút thay đổi nhanh linh hoạt.
*   🌐 **Hệ Thống Liên Kết Mở Rộng:** Tổng hợp danh sách các trang web chuyên đề tu tập, kinh điển, dự báo thời tiết (Windy) và các thông điệp tâm linh độc quyền.
*   🌙 **Giao Diện Dark Mode Hiện Phái:** Tông màu tối dịu mắt (`#0f172a`), điểm xuyết màu vàng kim (`#f59e0b`) tạo cảm giác tĩnh tại, trang nghiêm và hiện đại.

---

## 🛠️ Công Nghệ Sử Dụng

*   **HTML5 & CSS3** (Flexbox, CSS Variables, Responsive Design)
*   **JavaScript (Vanilla ES6+)** quản lý trạng thái (`localStorage`, DOM manipulation, Randomizer)
*   **FontAwesome 6.4.0** (Hệ thống biểu tượng trực quan)
*   **Google Fonts** (`Inter` cho giao diện sạch sẽ, `Lora` cho văn bản mang phong cách cổ điển/tâm linh)

---

## 📂 Cấu Trúc Mã Nguồn (`index.html`)

Toàn bộ ứng dụng được tối ưu đóng gói gọn trong một tệp duy nhất (`index.html`), giúp dễ dàng triển khai nhanh chóng lên **GitHub Pages**:

```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Trạm Phước Đức - Tâm Linh Modern</title>
    <!-- Styles & Fonts -->
</head>
<body>
    <div class="app-container">
        <!-- Header, Widget, Panel Tích Phước, Danh Ngôn, Liên Kết, Footer -->
    </div>
    <script>
        // Logic JavaScript xử lý bộ đếm, ngày tháng và lời khuyên
    </script>
</body>
</html>
