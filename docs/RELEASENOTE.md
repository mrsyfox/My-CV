# Release Notes - Website Portfolio CV Cá Nhân

---

## 📌 Thông Tin Phiên Bản

- **Phiên bản:** `v1.0`
- **Ngày phát hành:** 05/11/2026
- **Tác giả:** Nguyễn Đức Minh
- **Trạng thái:** Bản phát hành đầu tiên (First Official Release)
- **Công nghệ cốt lõi:** HTML5 Ngữ nghĩa (Semantic HTML) & CSS3 (Flexbox, CSS Grid)

---

## 🚀 Chức Năng Mới (New Features)

### 1. Nhận diện thương hiệu & Khu vực Giới thiệu (Header & Hero Section)
- **Header cố định & Điều hướng:** Thanh điều hướng trên cùng với logo cá nhân, menu điều hướng nhanh (smooth scroll) chuyển đến các phần: *Giới thiệu*, *Kỹ năng*, *Dự án*, *Liên hệ*.
- **Hero Banner chuyên nghiệp:** Trình bày họ tên, định hướng nghề nghiệp (Full-stack Developer & Cybersecurity), đoạn giới thiệu bản thân và ảnh đại diện chân dung.
- **Nút kêu gọi hành động (Call to Action):** 2 nút nổi bật "Xem dự án" và "Liên hệ tôi" giúp chuyển nhanh đến các khu vực trọng tâm.

### 2. Trình bày Kỹ năng (Skills Section)
- **Danh sách kỹ năng dạng thẻ (Skill Chips):** Trình bày trực quan các kỹ năng chuyên môn và thế mạnh cá nhân bao gồm: Python, HTML5, CSS3 / Flexbox / Grid, Photoshop, Guitar, Translation Skills.
- **Bố cục Flexbox co giãn:** Tự động điều chỉnh khoảng cách và xuống dòng mượt mà trên mọi độ phân giải màn hình.

### 3. Lưới Dự án & Thành tựu tiêu biểu (Projects Grid)
- **Bố cục CSS Grid Responsive:** Tự động co giãn theo 3 cấp độ màn hình: 1 cột (Mobile), 2 cột (Tablet), 3 cột (Desktop).
- **Thẻ dự án/thành tựu chi tiết (`<article class="card">`):**
  - **Chứng chỉ học thuật:** IELTS, giải học sinh giỏi, thư giới thiệu.
  - **Chứng chỉ âm nhạc & giải thưởng:** Chứng chỉ trung cấp 7 năm, các giải thưởng âm nhạc.
  - **Chứng nhận hoạt động ngoại khóa:** Dự án truyền bá văn hóa, tình nguyện, hội họa, học thuật, âm nhạc.
  - **Giải thưởng thể thao:** Giải bóng đá, điền kinh.
- **Hiển thị hình ảnh minh họa thực tế:** Đi kèm các thẻ gắn nhãn phân loại (tag list) rõ ràng.

### 4. Khu vực Liên hệ & Biểu mẫu (Contact Section)
- **Kênh kết nối mạng xã hội:** Cung cấp thông tin liên hệ trực tiếp qua Email, GitHub (`mrsyfox`), và Instagram cá nhân (`mr.syfoxowo`).
- **Biểu mẫu gửi tin nhắn (Contact Form):**
  - Các trường nhập liệu: *Họ và tên*, *Email*, *Lời nhắn* có thuộc tính HTML5 `required` bắt buộc nhập.
  - Tích hợp phương thức gửi thư qua giao thức `mailto:ducminhaha@gmail.com` với `enctype="text/plain"`.

### 5. Thiết kế Responsive Mobile-First & Chuẩn HTML5 Semantics
- **Mobile-First Workflow:** Tối ưu hóa kích thước màn hình nhỏ (360px) trước, sau đó mở rộng cho Tablet (768px) và Desktop (1280px+).
- **Không tràn màn hình:** Không phát sinh thanh cuộn ngang (horizontal scrollbar) ở bất kỳ độ phân giải nào.
- **HTML5 ngữ nghĩa đầy đủ:** Sử dụng chính xác các thẻ `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`.
- **Khả năng tiếp cận (Accessibility - a11y):** Thuộc tính `aria-label`, `alt` đầy đủ cho mọi hình ảnh, hỗ trợ điều hướng bằng bàn phím với hiệu ứng `focus-visible`.

### 6. Tài liệu & Môi trường chạy thử (Documentation & Dev Environment)
- Tệp `README.md` hướng dẫn chi tiết cách chạy dự án bằng nhiều phương pháp: mở trực tiếp, Live Server VS Code (cổng 5501), Python HTTP Server, và triển khai container qua Docker Nginx.

---

## 🛠 Lỗi Đã Sửa (Bug Fixes)

Trong quá trình hoàn thiện phiên bản v1.0, các lỗi và điểm bất cập từ bản mẫu ban đầu đã được kiểm tra và xử lý triệt để:

1. **Sửa thông tin định danh và quyền tác giả:**
   - Thay đổi thẻ `<meta name="author" content="Nguyễn Văn An" />` thành `Nguyễn Đức Minh`.
   - Cập nhật thông tin bản quyền footer và tiêu đề trang tương ứng.
2. **Sửa lỗi chính tả trong văn bản (Content Typo):**
   - Đã sửa từ khóa nghề nghiệp `"cyber cercuity"` thành `"cybersecurity"` trong đoạn văn giới thiệu mục tiêu nghề nghiệp tại phần Hero.
3. **Cập nhật chính xác thuộc tính `alt` của hình ảnh:**
   - Thay thế các đoạn văn bản `alt` mặc định từ mẫu (như *"Ảnh minh họa dự án Landing Page"*, *"Todo App"*, *"Weather Dashboard"*, *"Blog cá nhân"*) thành mô tả chính xác nội dung ảnh thực tế (*"Ảnh minh họa chứng chỉ học thuật"*, *"Ảnh minh họa chứng chỉ âm nhạc và giải thưởng"*, v.v.). Giúp cải thiện khả năng tiếp cận (screen reader) và chuẩn SEO.
4. **Loại bỏ các liên kết rác / liên kết chết (Dead Links):**
   - Loại bỏ các thẻ `<a class="card-link" href="#">Xem chi tiết →</a>` chưa có trang đích thực tế trong các thẻ dự án, tránh gây hiểu lầm hoặc trải nghiệm người dùng không tốt khi nhấp vào.
5. **Khắc phục lỗi biểu mẫu liên hệ không gửi được dữ liệu:**
   - Bổ sung `action="mailto:ducminhaha@gmail.com"`, `method="post"`, `enctype="text/plain"` cho thẻ `<form>`.
   - Bổ sung thuộc tính `name` (`name="name"`, `name="email"`, `name="message"`) cho các trường `input` và `textarea`, khắc phục lỗi biểu mẫu không đóng gói được dữ liệu khi submit.
6. **Sửa lỗi cú pháp CSS không hợp lệ:**
   - Sửa lỗi cú pháp màu sắc `color: #white;` trên nút gửi tin nhắn thành giá trị màu hợp lệ `color: #fff;`.

---

## ⚠️ Hạn Chế Còn Tồn Tại (Known Limitations)

Mặc dù phiên bản v1.0 đã đáp ứng đầy đủ các tiêu chí kỹ thuật và giao diện cơ bản của một Portfolio cá nhân, hiện vẫn còn một số điểm hạn chế dự kiến sẽ được nâng cấp trong các phiên bản tiếp theo:

1. **Biểu mẫu liên hệ phụ thuộc Email Client máy người dùng:**
   - Hiện tại form gửi thư thông qua giao thức `mailto:`, yêu cầu thiết bị của người dùng phải cài đặt và cấu hình sẵn ứng dụng mail mặc định (như Outlook, Mail app, hoặc webmail).
   - *Hướng phát triển v1.1:* Tích hợp Backend API (Node.js/Express) hoặc các dịch vụ form handling của bên thứ ba (EmailJS, Formspree, Resend) để gửi thư tự động trong nền mà không cần mở ứng dụng ngoài.
2. **Chưa có trang nội dung chi tiết cho từng chứng chỉ / dự án:**
   - Các thẻ thành tựu mới chỉ hiển thị bản tóm tắt và ảnh bìa thu nhỏ. Chưa có modal popup phóng to ảnh chứng chỉ hoặc đường dẫn sang trang chi tiết để xem hồ sơ đính kèm.
   - *Hướng phát triển v1.1:* Bổ sung lightbox/modal preview xem ảnh gốc kích thước lớn và các tệp PDF chứng chỉ đính kèm.
3. **Chưa tích hợp chế độ Sáng / Tối (Dark/Light Mode Toggle):**
   - Giao diện hiện tại cố định ở tông màu tối (Dark theme hiện đại), chưa có nút gạt cho phép người dùng tùy chọn chuyển đổi sang giao diện sáng (Light theme).
4. **Chưa có hiệu ứng tương tác nâng cao bằng JavaScript:**
   - Website hoàn toàn xây dựng bằng HTML và CSS thuần túy, chưa có hiệu ứng cuộn trang mượt mà tùy biến (Scroll animations / AOS), kiểm tra hợp lệ dữ liệu biểu mẫu trực tiếp trên giao diện (Realtime Form Validation), hay menu hamburger có hiệu ứng đóng mở trượt trên thiết bị di động nhỏ.
5. **Chưa hỗ trợ đa ngôn ngữ (Internationalization - i18n):**
   - Nội dung website hiện tại chỉ có phiên bản tiếng Việt (`lang="vi"`), chưa có tính năng chuyển đổi ngôn ngữ Việt - Anh phục vụ nhà tuyển dụng nước ngoài.

---
*Bản quyền ghi nhận © 2026 Nguyễn Đức Minh. Mọi đóng góp và phản hồi vui lòng gửi về email: ducminhaha@gmail.com.*

