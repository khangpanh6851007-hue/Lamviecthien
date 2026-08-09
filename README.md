# Trạm Phước Đức - Tâm Linh Modern 🌟

<div align="center">

![GitHub Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![GitHub Version](https://img.shields.io/badge/Version-2026.1.0-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Web%20%2F%20Mobile-orange?style=for-the-badge)

*Hệ thống hỗ trợ tu tâm tích phước hằng ngày, thiết kế hiện đại, tối ưu trải nghiệm trên mọi thiết bị.*

</div>

---

## 📌 Giới Thiệu Dự Án

**Trạm Phước Đức** là một ứng dụng web tâm linh hiện đại, được xây dựng nhằm giúp người dùng dễ dàng thực hành tu dưỡng thân tâm, tích lũy phước đức hằng ngày, theo dõi đồng hồ thời gian thực, đếm ngược các mốc quan trọng và truy cập nhanh chóng vào kho tàng các bài đọc, kinh sách, tư tưởng tâm linh.

---

## ✨ Tính Năng Nổi Bật (2026 Edition)

- 🕒 **Đồng Hồ & Ngày Tháng Thời Gian Thực:** Cập nhật chính xác lịch âm/dương và giờ giấc trực tiếp theo thời gian hệ thống.
- ⏳ **Đếm Ngược 100 Năm Ân Xá Nhân Loại:** Theo dõi chi tiết từng năm, ngày, giờ, giây của chu kỳ ân xá đặc biệt.
- 🙏 **Gieo Duyên Lành (Tích Phước):** Nút tương tác niệm câu lành với bộ nhớ `localStorage` tự động lưu lại tổng số niệm tích lũy cá nhân.
- 📖 **Lời Khuyên Tâm Linh Ngẫu nhiên:** Hệ thống gợi ý câu nói, lời khuyên giúp tâm hồn an tịnh mỗi ngày.
- 🔗 **Thư Viện Liên Kết Phong Phú:** Truy cập nhanh đến các trạm chủ đề như *Nam Mô Đại Bi Quán Thế Âm Bồ Tát*, *Sấm Trạng Trình*, *Cung Trời Hóa Lạc*, *Tây Phương Cực Lạc*, *Thời Kỳ Mạt Pháp*, v.v.

---

## 🚀 Cấu Trúc Mã Nguồn (Single-File App)

Dự án sử dụng cấu trúc gọn nhẹ với một file `index.html` duy nhất chứa đầy đủ HTML5, CSS3 (Flexbox/Grid, Responsive Variables) và Vanilla JavaScript:

```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Trạm Phước Đức - Tâm Linh Modern</title>
    <!-- Import Google Fonts & FontAwesome Icons -->
    ...
</head>
<body>
    <!-- App Container -->
    <div class="app-container">
        <!-- Header, Widgets, Countdown, Blessing Panel, Links & Footer -->
    </div>
    <script>
        // Logic JS quản lý thời gian, đếm ngược, localStorage và sự kiện tương tác
    </script>
</body>
</html>
