# IELTS with Vy - Landing Page

Một landing page tĩnh (Single-page) được thiết kế theo phong cách **"Apple Liquid Glass"** (Kính trong suốt) dành cho lớp học IELTS của cô Vy (Pzy). Trang web tập trung mang lại trải nghiệm người dùng (UX) cực kỳ mượt mà, hiệu ứng thị giác sang trọng, tinh tế nhưng vẫn đảm bảo tối ưu hóa hiệu năng phần cứng xuất sắc (duy trì 60fps trên cả thiết bị di động).

## ✨ Tính năng nổi bật

* **Giao diện Apple Liquid Glass:** Thay vì dùng frosted glass thông thường, trang web sử dụng sự kết hợp giữa độ mờ (`blur`), độ bão hòa (`saturate`) và các lớp viền (rim) đa tầng để tạo ra hiệu ứng kính có độ sâu, trong vắt và khúc xạ ánh sáng chân thực mang hơi hướng iOS/macOS.
* **Hiệu ứng tương tác mượt mà (60fps):** * Hiệu ứng đánh máy (Typing effect) mượt mà ở phần Hero.
    * **Nút bấm từ tính (Magnetic buttons)** bám theo con trỏ chuột trên desktop.
    * Hiệu ứng ánh sáng lướt qua thẻ (Glare effect) khi di chuột.
    * Glow bám theo con trỏ chuột (ambient cursor glow).
    * Hiệu ứng cuộn trang (Scroll reveal) xuất hiện uyển chuyển.
* **Accordion Hiệu năng cao:** Lộ trình học được đóng gói trong Accordion tối ưu hóa đặc biệt. Sử dụng CSS Grid (`grid-template-rows`) và **View Transitions API** giúp thao tác đóng/mở mượt mà, không bị giật lag khung hình.
* **Video Player Tùy chỉnh (Custom UI):** Trình phát video được tích hợp sẵn giao diện kính, hỗ trợ thanh tua (scrubber), bật/tắt tiếng và tự động phát/tạm dừng (Intersection Observer) khi cuộn trang để tiết kiệm tài nguyên.
* **Form Đăng ký Sống động:** Form Validate trực tiếp, hiệu ứng rung (shake) khi nhập thiếu thông tin và hiệu ứng tung pháo giấy (confetti) thú vị khi gửi thành công.
* **Nền Voronoi Động:** Background sử dụng SVG filter `feTurbulence` nhẹ nhàng, tạo cảm giác chuyển động vân lỏng sống động mà không tốn tài nguyên chạy JavaScript canvas.

## 🛠 Công nghệ sử dụng

* **HTML5 / CSS3 / Vanilla JavaScript:** Code thuần, không phụ thuộc vào các framework JS nặng nề (React/Vue).
* **Tailwind CSS (CDN):** Hỗ trợ thiết lập layout và chia lưới (grid/flexbox) nhanh chóng.
* **CSS View Transitions API:** Xử lý hiệu ứng chuyển trạng thái mượt mà bằng GPU.
* **CSS Variables (Custom Properties):** Quản lý toàn bộ Design Tokens tập trung tại `:root`.

## 📂 Cấu trúc dự án

Dự án có cấu trúc vô cùng tối giản, dễ dàng deploy lên mọi nền tảng hosting tĩnh (GitHub Pages, Vercel, Netlify...):

```text
├── assets/
│   ├── idp-ielts-lockup.png      # Logo đối tác IDP
│   ├── idp-ielts-partnership.png
│   ├── idp-ielts-referral.png
│   ├── idp-logo.png
│   ├── ielts-persons-logo.png    # Logo IELTS Persons
│   ├── lens-displacement.png     # Map khúc xạ cho SVG filters
│   ├── logo-circle.png           
│   ├── vy-hero.jpg               # Ảnh hero chân dung
│   ├── vy-portrait-1.jpg
│   ├── vy-portrait-2.jpg
│   └── class-clip.mp4            # Video clip lớp học
├── index.html                    # File giao diện chính (chứa HTML, cấu hình Tailwind, CSS, JS)
└── README.md                     # Tài liệu hướng dẫn
