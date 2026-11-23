# 🔍 CFV — CodeFlow Visualizer & Security Lab Sandbox

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-GitHub_Pages-0284c7?style=for-the-badge)](https://z3r0d4y-007.github.io/codeflow-visualizer/)
[![License: MIT](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge)](LICENSE)
[![Zero Setup](https://img.shields.io/badge/Setup-100%25_Client--Side_HTML-a78bfa?style=for-the-badge)](#)

**CFV (CodeFlow Visualizer)** là công cụ trực quan hóa luồng dữ liệu mã nguồn 2 chiều (**Source ➔ Filter ➔ Sink ➔ Return**) kết hợp với **Mini Burp Suite (Repeater, Proxy & Optional Intercept, Intruder)** và **Interactive Browser Sandbox** ngay trên một giao diện duy nhất — không cần cài đặt server hay cấu hình proxy phức tạp.

👉 **Trải nghiệm trực tuyến ngay tại:** **[https://z3r0d4y-007.github.io/codeflow-visualizer/](https://z3r0d4y-007.github.io/codeflow-visualizer/)**

---

## ✨ Tính năng nổi bật

| Tính năng | Mô tả chi tiết |
| :--- | :--- |
| **🗺️ Sơ đồ Luồng dữ liệu 2 chiều** | Tự động phân tích mã nguồn (Python/Flask, JavaScript, HTML/HTTP Raw) thành sơ đồ 4 cột trực quan, liên kết 2 chiều với từng dòng code bên trái và truy vết ngược nguyên nhân câu lệnh `return`. |
| **📌 Theo dõi Biến Ghi & Hiển thị** | Tự động phát hiện và tô sáng các biến toàn cục / trạng thái do người dùng ghi vào và được hiển thị ngược lại qua các route khác nhau. |
| **🧪 Repeater & Browser Render** | Giao diện chia 2 cột đối xứng chuẩn Burp Suite: chỉnh sửa **Raw HTTP Request** bên trái, xem **Raw HTTP Response** và kết xuất trực tiếp trên **Browser Render** bên phải. |
| **🌐 Proxy History & Intercept** | Tự động ghi lại toàn bộ gói tin từ thanh địa chỉ Browser hoặc Repeater vào **Proxy History**. Hỗ trợ nút bật/tắt **Intercept (On / Off)** tùy chọn để giữ và chỉnh sửa gói tin trước khi *Forward* hoặc *Drop*. |
| **🎯 Intruder QA Matrix** | Chạy kiểm thử tổ hợp tham số (`Sniper`, `Battering Ram`, `Pitchfork`, `Cluster Bomb`) ngay trong sandbox và đối chiếu sơ đồ luồng của từng lượt chạy. |
| **📡 Virtual Webhook & Link Test** | Tạo link kiểm thử nhanh và đồng bộ nhật ký callback theo thời gian thực giữa các tab trình duyệt. |

---

## 🚀 Cách sử dụng

1. Truy cập **[Live Demo](https://z3r0d4y-007.github.io/codeflow-visualizer/)** hoặc tải tệp `index.html` về mở trực tiếp trên trình duyệt.
2. Chọn một trong **7 bài Lab mẫu** ở góc trên bên trái (hoặc chuyển sang tab **✏️ Sửa / Dán Code** để dán mã nguồn của bạn rồi bấm **⚡ Phân tích Code**).
3. Bấm vào từng khối trên sơ đồ để xem dòng code tương ứng, điều kiện rẽ nhánh và cảnh báo rủi ro.
4. Chuyển sang tab **🧪 Repeater & Browser** hoặc **🌐 Proxy & Intercept** để gửi gói tin, nhập URL lên thanh địa chỉ trình duyệt và quan sát luồng thực thi.

---

## 🛠️ Công nghệ sử dụng

- **Core:** Vanilla HTML5, CSS3, JavaScript (ES6+) — đóng gói gọn nhẹ trong 1 tệp duy nhất, hoạt động hoàn toàn phía client.
- **Visualization:** Custom SVG Bezier Edge Renderer kết hợp Pan/Zoom Canvas.

---

## 🤝 Đóng góp & Góp ý

Dự án vẫn đang trong quá trình phát triển và hoàn thiện. Nếu bạn phát hiện lỗi hoặc có ý tưởng nâng cấp (như hỗ trợ thêm ngôn ngữ lập trình, AST parser hoặc bài Lab mẫu mới), hãy mở một **Issue** hoặc gửi **Pull Request** nhé!
