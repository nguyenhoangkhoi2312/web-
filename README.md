# IELTS with Vy - Landing Page

Một landing page tĩnh được thiết kế theo phong cách **"Apple Liquid Glass"** dành cho lớp học IELTS của Pzy. 

## ✨ Tính năng nổi bật

* **Giao diện Apple Liquid Glass:** Thay vì dùng frosted glass thông thường, trang web sử dụng sự kết hợp giữa độ mờ (`blur`), độ bão hòa (`saturate`) và các lớp viền đa tầng để tạo ra hiệu ứng kính có độ sâu, trong vắt và khúc xạ ánh sáng chân thực mang hơi hướng iOS/macOS.
    * **Magnetic buttons** bám theo con trỏ chuột trên desktop.
    * Glare effect khi di chuột.
    * ambient cursor glow.
    * Scroll reveal.
* **Accordion Hiệu năng cao:** Lộ trình học được đóng gói trong Accordion. Sử dụng CSS Grid (`grid-template-rows`) và **View Transitions API** giúp thao tác đóng/mở mượt.
* **Video Player:** Trình phát video được tích hợp sẵn giao diện kính, hỗ trợ scrubber, bật/tắt tiếng và tự động phát/tạm dừng khi cuộn trang để tiết kiệm tài nguyên.
* **Form Đăng ký Sống động:** Form Validate trực tiếp, hiệu ứng rung (shake) khi nhập thiếu thông tin và hiệu ứng tung pháo giấy (confetti) thú vị khi gửi thành công.
* **Nền Voronoi Động:** Background sử dụng SVG filter `feTurbulence` nhẹ nhàng, tạo cảm giác chuyển động vân lỏng sống động mà không tốn tài nguyên chạy JavaScript canvas.

## 🛠 Công nghệ sử dụng

* **HTML5 / CSS3 / Vanilla JavaScript** 
* **Tailwind CSS (CDN)** 
* **CSS View Transitions API** 
* **CSS Variables (Custom Properties)** 

## 📂 Cấu trúc dự án


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
