# 🌟 Trạm Phước Đức - Tâm Linh Modern

Hệ thống ứng dụng web hiện đại hỗ trợ tu tâm, tích phước, theo dõi thời gian thực và đếm ngược chu kỳ ân xá cho toàn thể nhân loại. 

Được thiết kế tối ưu hóa giao diện hoàn hảo cho nền tảng di động và máy tính bảng, tương thích tuyệt vời trên các môi trường soạn thảo mã nguồn như **Acode** hoặc **Ameba/Aedit (Trebuchet/Acode)**.

---

## 🚀 Tính Năng Nổi Bật

*   🕒 **Đồng Hồ & Lịch Trực Tuyến:** Hiển thị thời gian thực (Giờ:Phút:Giây) kết hợp cùng lịch ngày tháng năm linh hoạt.
*   ⏳ **Đếm Ngược 100 Năm Ân Xá:** Theo dõi chính xác thời gian còn lại của chu kỳ 100 năm ân xá cho toàn thể nhân loại tính đến mốc thời gian chuyển giao.
*   🙏 **Gieo Duyên Lành Hằng Ngày:** Nút tương tác niệm câu lành tích lũy số lượng cá nhân hóa lưu trữ trực tiếp bằng `localStorage`.
*   📜 **Lời Khuyên Tâm Linh:** Kho tàng các câu châm ngôn, lời nhắc nhở hướng thiện tự động làm mới hoặc thay đổi linh hoạt.
*   🌐 **Hệ Thống Liên Kết Tâm Linh:** Tích hợp bộ sưu tập các đường dẫn nhanh đến các không gian tài nguyên, sấm trạng, cõi trời hóa lạc, mạt pháp và thượng ngươn thánh đức.

---

## 🛠️ Hướng Dẫn Sử Dụng & Đưa Lên GitHub (2026)

Để chạy file này trên ứng dụng **Acode** / **Trebuchet (Trebedit)** và đưa lên kho lưu trữ **GitHub**, bạn thực hiện theo các bước đơn giản sau:

### Bước 1: Tạo và Chạy trên Acode / Trebedit
1. Mở ứng dụng **Acode** hoặc **Trebedit** trên thiết bị di động của bạn.
2. Tạo một file mới hoàn toàn và đặt tên là `index.html`.
3. Sao chép toàn bộ mã nguồn HTML ở phần bên dưới dán vào file `index.html`.
4. Nhấn nút **Play / Preview** bên trong ứng dụng để kiểm tra trực tiếp giao diện trên trình duyệt di động.

### Bước 2: Đẩy Lên GitHub Pages
1. Truy cập vào [GitHub](https://github.com) và tạo một Repository mới (ví dụ đặt tên: `tramphuocduc`).
2. Tải file `index.html` lên repository vừa tạo (hoặc kết nối Git qua terminal/Acode git plugin).
3. Vào phần **Settings** của repository -> Chọn **Pages**.
4. Tại mục **Build and deployment**, phần *Branch* chọn `main` (hoặc `master`) và chọn `/root`, sau đó nhấn **Save**.
5. Chờ khoảng 1-2 phút, GitHub sẽ cung cấp cho bạn một đường dẫn trực tuyến công khai để chia sẻ với mọi người.

---

## 💻 Mã Nguồn Hoàn Chỉnh (`index.html`)

```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Trạm Phước Đức - Tâm Linh Modern</title>
    <!-- Google Fonts -->
    <link href="[https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Lora:ital,wght@0,500;1,500&display=swap](https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Lora:ital,wght@0,500;1,500&display=swap)" rel="stylesheet">
    <!-- FontAwesome Icon -->
    <link rel="stylesheet" href="[https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css)">
    <style>
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --accent-gold: #f59e0b;
            --text-main: #f8fafc;
            --text-sub: #94a3b8;
            --border-color: rgba(245, 158, 11, 0.2);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 16px;
        }

        .app-container {
            width: 100%;
            max-width: 440px;
            background: var(--card-bg);
            border-radius: 20px;
            border: 1px solid var(--border-color);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.5);
            padding: 20px;
        }

        /* Header */
        .app-header {
            text-align: center;
            margin-bottom: 20px;
        }
        .app-header h1 {
            font-size: 18px;
            font-weight: 700;
            color: var(--accent-gold);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 4px;
        }
        .app-header p {
            font-size: 12px;
            color: var(--text-sub);
        }

        /* Widget Đồng Hồ & Ngày Tháng */
        .widget-box {
            background: rgba(15, 23, 42, 0.6);
            border-radius: 12px;
            padding: 12px 16px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 16px;
            font-size: 13px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        .widget-box span i {
            color: var(--accent-gold);
            margin-right: 6px;
        }
        .live-clock {
            font-weight: 600;
            color: var(--accent-gold);
        }

        /* Panel Đếm Ngược 100 Năm Ân Xá */
        .amnesty-countdown-panel {
            background: linear-gradient(135deg, rgba(239, 68, 68, 0.1), rgba(30, 41, 59, 0.8));
            border: 1px solid rgba(239, 68, 68, 0.3);
            border-radius: 14px;
            padding: 16px;
            text-align: center;
            margin-bottom: 16px;
        }
        .amnesty-countdown-panel h3 {
            font-size: 13px;
            font-weight: 600;
            margin-bottom: 10px;
            color: #fca5a5;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        .countdown-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 6px;
            margin-top: 8px;
        }
        .countdown-item {
            background: rgba(15, 23, 42, 0.7);
            border: 1px solid rgba(239, 68, 68, 0.2);
            border-radius: 8px;
            padding: 8px 4px;
        }
        .countdown-value {
            font-size: 15px;
            font-weight: 700;
            color: var(--text-main);
        }
        .countdown-label {
            font-size: 9px;
            color: var(--text-sub);
            text-transform: uppercase;
            margin-top: 2px;
        }

        /* Tính năng Tích Phước Mới */
        .blessing-panel {
            background: linear-gradient(135deg, rgba(245, 158, 11, 0.1), rgba(30, 41, 59, 0.8));
            border: 1px solid var(--border-color);
            border-radius: 14px;
            padding: 18px;
            text-align: center;
            margin-bottom: 16px;
        }
        .blessing-panel h3 {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 10px;
            color: #fde68a;
        }
        .action-btn {
            background: var(--accent-gold);
            color: #0f172a;
            border: none;
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: 700;
            font-size: 13px;
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            box-shadow: 0 4px 12px rgba(245, 158, 11, 0.3);
            transition: transform 0.1s;
        }
        .action-btn:active {
            transform: scale(0.95);
        }
        .counter-display {
            margin-top: 10px;
            font-size: 12px;
            color: var(--text-sub);
        }
        .counter-display b {
            color: var(--accent-gold);
        }

        /* Lời Khuyên Tâm Linh */
        .advice-box {
            background: rgba(15, 23, 42, 0.4);
            border-left: 3px solid var(--accent-gold);
            padding: 12px 14px;
            border-radius: 0 10px 10px 0;
            margin-bottom: 16px;
        }
        .advice-text {
            font-family: 'Lora', serif;
            font-style: italic;
            font-size: 13px;
            line-height: 1.4;
            color: #e2e8f0;
            margin-bottom: 6px;
        }
        .advice-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 11px;
            color: var(--text-sub);
        }
        .change-advice-btn {
            background: none;
            border: none;
            color: var(--accent-gold);
            cursor: pointer;
            font-size: 11px;
            font-weight: 600;
        }

        /* Danh Sách Liên Kết Web */
        .nav-links {
            display: flex;
            flex-direction: column;
            gap: 8px;
            max-height: 220px;
            overflow-y: auto;
            padding-right: 2px;
        }
        .nav-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: rgba(15, 23, 42, 0.5);
            padding: 10px 14px;
            border-radius: 10px;
            color: var(--text-main);
            text-decoration: none;
            font-size: 13px;
            font-weight: 500;
            border: 1px solid rgba(255, 255, 255, 0.04);
            transition: background 0.2s;
        }
        .nav-item:hover, .nav-item:active {
            background: rgba(245, 158, 11, 0.1);
            border-color: var(--border-color);
        }
        .nav-item span {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .nav-item i.fa-solid {
            color: var(--accent-gold);
        }
        .nav-item .fa-chevron-right {
            font-size: 10px;
            color: var(--text-sub);
        }

        /* Footer */
        .app-footer {
            text-align: center;
            margin-top: 16px;
            font-size: 10px;
            color: var(--text-sub);
        }
        .app-footer span {
            color: var(--accent-gold);
        }
    </style>
</head>
<body>

    <div class="app-container">
        <!-- Tiêu đề -->
        <div class="app-header">
            <h1>Trạm Phước Đức</h1>
            <p>Hệ thống hỗ trợ tu tâm tích phước hằng ngày</p>
        </div>

        <!-- Widget Đồng Hồ & Ngày Tháng -->
        <div class="widget-box">
            <span id="dateDisplay"><i class="fa-solid fa-calendar-day"></i> Đang cập nhật...</span>
            <span class="live-clock" id="liveClock"><i class="fa-solid fa-clock"></i> 00:00:00</span>
        </div>

        <!-- Panel Đếm Ngược 100 Năm Ân Xá Nhân Loại -->
        <div class="amnesty-countdown-panel">
            <h3><i class="fa-solid fa-hourglass-end"></i> Đếm Ngược 100 Năm Ân Xá Nhân Loại</h3>
            <div class="countdown-grid">
                <div class="countdown-item">
                    <div class="countdown-value" id="cdYears">00</div>
                    <div class="countdown-label">Năm</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-value" id="cdDays">00</div>
                    <div class="countdown-label">Ngày</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-value" id="cdHours">00</div>
                    <div class="countdown-label">Giờ</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-value" id="cdSecs">00</div>
                    <div class="countdown-label">Giây</div>
                </div>
            </div>
        </div>

        <!-- Nút Tích Phước -->
        <div class="blessing-panel">
            <h3>Gieo Duyên Lành Hằng Ngày</h3>
            <button class="action-btn" id="blessingBtn" type="button">
                <i class="fa-solid fa-hands-praying"></i> Niệm 1 Câu Lành
            </button>
            <div class="counter-display">Tổng số niệm lành đã tích lũy: <b id="countDisplay">0</b></div>
        </div>

        <!-- Lời Khuyên -->
        <div class="advice-box">
            <div class="advice-text" id="adviceText">"Tâm thiện hướng đi đâu cũng gặp bình an."</div>
            <div class="advice-footer">
                <span id="adviceAuthor">- Lời Nhủ</span>
                <button class="change-advice-btn" id="changeAdviceBtn" type="button">Đổi câu khác</button>
            </div>
        </div>

        <!-- Liên Kết Nhanh -->
        <div class="nav-links">
            <a href="[https://khangpanh6851007-hue.github.io/Linhhontrove/](https://khangpanh6851007-hue.github.io/Linhhontrove/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-unlock"></i> TỪNG PHẠT CHÚNG SINH -PHẠM LỖI KHÔNG SỬA</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://www.windy.com](https://www.windy.com)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-cloud-sun"></i> Windy Thời Tiết</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Samtrangtrinh/](https://khangpanh6851007-hue.github.io/Samtrangtrinh/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-book-reader"></i> Sấm Trạng Trình</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Cungtroihoalac/](https://khangpanh6851007-hue.github.io/Cungtroihoalac/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-cloud-moon"></i> Cung Trời Hóa Lạc</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Cungtroihoalacmobile/](https://khangpanh6851007-hue.github.io/Cungtroihoalacmobile/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-star"></i> Tích Đức Ở Cung Trời Hóa Lạc</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Ph-tth-chca-/](https://khangpanh6851007-hue.github.io/Ph-tth-chca-/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-om"></i> Tích Phước Cực Lạc</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Tayphuongcuclac](https://khangpanh6851007-hue.github.io/Tayphuongcuclac)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-place-of-worship"></i> Tây Phương Cực Lạc</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/CuocPhanxetcuoicung/](https://khangpanh6851007-hue.github.io/CuocPhanxetcuoicung/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-scale-balanced"></i> Cuộc Đại Phán Xét Cuối Cùng Của Nhân Loại</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Ng-c-/](https://khangpanh6851007-hue.github.io/Ng-c-/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-chess-king"></i> Ngọc Đế Ban Ân Xá</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Bangphongthan/](https://khangpanh6851007-hue.github.io/Bangphongthan/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-scroll"></i> Bảng Phong Thần</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Thoikymatphap/](https://khangpanh6851007-hue.github.io/Thoikymatphap/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-hourglass-half"></i> Thời Kỳ Mạt Pháp</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/Thuongnguonducthanh/](https://khangpanh6851007-hue.github.io/Thuongnguonducthanh/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-sun"></i> Thượng Ngươn Thánh Đức</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
            <a href="[https://khangpanh6851007-hue.github.io/10-i-uQuyYTamB-o-/](https://khangpanh6851007-hue.github.io/10-i-uQuyYTamB-o-/)" class="nav-item" target="_blank">
                <span><i class="fa-solid fa-book-bookmark"></i> 10 Điều Quy Y Tam Bảo</span>
                <i class="fa-solid fa-chevron-right"></i>
            </a>
        </div>

        <div class="app-footer">
            Thiết kế dành riêng cho <span>KhangPanh68</span>
        </div>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            // --- 1. ĐỒNG HỒ TỰ ĐỘNG & NGÀY THÁNG ---
            const now = new Date();
            const dateString = now.toLocaleDateString('vi-VN', { weekday: 'long', year: 'numeric', month: 'numeric', day: 'numeric' });
            const dateDisplay = document.getElementById('dateDisplay');
            if (dateDisplay) dateDisplay.innerHTML = `<i class="fa-solid fa-calendar-day"></i> ${dateString}`;

            const liveClock = document.getElementById('liveClock');
            function updateClock() {
                const d = new Date();
                const hours = String(d.getHours()).padStart(2, '0');
                const minutes = String(d.getMinutes()).padStart(2, '0');
                const seconds = String(d.getSeconds()).padStart(2, '0');
                if (liveClock) {
                    liveClock.innerHTML = `<i class="fa-solid fa-clock"></i> ${hours}:${minutes}:${seconds}`;
                }
            }
            setInterval(updateClock, 1000);
            updateClock();

            // --- 2. ĐẾM NGƯỢC 100 NĂM ÂN XÁ CHO TOÀN THỂ NHÂN LOẠI ---
            const amnestyTargetDate = new Date("December 31, 2124 23:59:59").getTime();

            const cdYears = document.getElementById('cdYears');
            const cdDays = document.getElementById('cdDays');
            const cdHours = document.getElementById('cdHours');
            const cdSecs = document.getElementById('cdSecs');

            function updateAmnestyCountdown() {
                const currentTime = new Date().getTime();
                const timeLeft = amnestyTargetDate - currentTime;

                if (timeLeft > 0) {
                    const totalSeconds = Math.floor(timeLeft / 1000);
                    const years = Math.floor(totalSeconds / (3600 * 24 * 365));
                    const days = Math.floor((totalSeconds % (3600 * 24 * 365)) / (3600 * 24));
                    const hours = Math.floor((totalSeconds % (3600 * 24)) / 3600);
                    const seconds = totalSeconds % 60;

                    if (cdYears) cdYears.innerText = String(years).padStart(2, '0');
                    if (cdDays) cdDays.innerText = String(days).padStart(3, '0');
                    if (cdHours) cdHours.innerText = String(hours).padStart(2, '0');
                    if (cdSecs) cdSecs.innerText = String(seconds).padStart(2, '0');
                } else {
                    if (cdYears) cdYears.innerText = "00";
                    if (cdDays) cdDays.innerText = "000";
                    if (cdHours) cdHours.innerText = "00";
                    if (cdSecs) cdSecs.innerText = "00";
                }
            }
            setInterval(updateAmnestyCountdown, 1000);
            updateAmnestyCountdown();

            // --- 3. TÍNH NĂNG TÍCH PHƯỚC ---
            let count = parseInt(localStorage.getItem('tram_phuoc_duc_count')) || 108;
            const countDisplay = document.getElementById('countDisplay');
            const blessingBtn = document.getElementById('blessing