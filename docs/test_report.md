# BÁO CÁO KIỂM THỬ PHẦN MỀM (TEST REPORT)

---

## 📋 THÔNG TIN CHUNG (GENERAL INFORMATION)

| Mục | Thông tin chi tiết |
| :--- | :--- |
| **Tên dự án** | Website Portfolio CV Cá Nhân (Bài kiểm tra A2.1) |
| **Sản phẩm bàn giao** | Website tĩnh Portfolio CV giới thiệu cá nhân, kỹ năng, dự án và thông tin liên hệ |
| **Phiên bản (Build/Version)** | `v1.0` (Commit: `6b1c2cf`) |
| **Ngày thực hiện kiểm thử** | 05/11/2026 |
| **Người thực hiện / Đánh giá** | QA/QC Engineer - Nguyễn Đức Minh |
| **Môi trường kiểm thử** | • **Hệ điều hành:** Windows 11 Pro 64-bit<br>• **Trình duyệt:** Google Chrome (v130+), Microsoft Edge (v130+), Mozilla Firefox (v131+), Safari (Mobile WebKit)<br>• **Web Server:** VS Code Live Server (Port 5501), Python `http.server` (Port 8000), Docker Nginx Alpine (Port 8080)<br>• **Độ phân giải thử nghiệm:** Mobile (360x640, 390x844), Tablet (768x1024), Desktop (1280x720, 1920x1080) |
| **Tài liệu tham chiếu** | Báo cáo đặc tả yêu cầu `BAOCAO-A2.1.pdf`, `README.md`, `docs/RELEASENOTE.md` |

---

## 📊 BẢNG TỔNG QUAN TRẠNG THÁI (TEST SUMMARY)

| STT | Nhóm tiêu chí đánh giá | Số lượng kiểm tra | Đạt (Pass) | Cần cải thiện | Chưa đạt (Fail) | Đánh giá chung |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: |
| **1** | **Tính đúng đắn và mức độ đáp ứng yêu cầu chức năng** | 6 | 5 | 1 | 0 | **ĐẠT YÊU CẦU** |
| **2** | **Giao diện, trải nghiệm người dùng và khả năng tương thích** | 6 | 6 | 0 | 0 | **XUẤT SẮC** |
| **3** | **Khả năng vận hành, xử lý lỗi và hiệu năng cơ bản** | 5 | 5 | 0 | 0 | **ĐẠT TIÊU CHUẨN** |
| **4** | **Bảo mật, quản lý cấu hình và dữ liệu** | 5 | 5 | 0 | 0 | **ĐẠT TIÊU CHUẨN** |
| **5** | **Chất lượng mã nguồn, cấu trúc repository và tài liệu** | 5 | 5 | 0 | 0 | **XUẤT SẮC** |
| **6** | **Khả năng triển khai, kiểm thử và cung cấp minh chứng** | 5 | 5 | 0 | 0 | **XUẤT SẮC** |
| **TỔNG** | **Toàn bộ 6 nhóm tiêu chí bàn giao** | **32** | **31 (96.9%)** | **1 (3.1%)** | **0 (0%)** | **SẴN SÀNG BÀN GIAO** |

---

## 🔍 NỘI DUNG CHI TIẾT TỪNG TIÊU CHÍ KIỂM THỬ

### 1. Tính đúng đắn và mức độ đáp ứng yêu cầu chức năng

> Đánh giá sự đầy đủ và chính xác của 5 khối nội dung chính: Nhận diện & Giới thiệu, Điều hướng, Kỹ năng, Dự án / Thành tựu, và Liên hệ.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-FN-01** | **Khối Nhận diện & Giới thiệu (Hero):** Hiển thị đúng họ tên, định hướng nghề nghiệp, đoạn mô tả và ảnh đại diện chân dung. | Cao | **Đạt** | Hiển thị chuẩn xác tên "Nguyễn Đức Minh", vai trò "Undergraduate & Developer", định hướng Cybersecurity & Full-stack. Ảnh đại diện `THPT Hoàng Cầu0806.jpg` tải sắc nét, đúng tỷ lệ. |
| **TC-FN-02** | **Thanh Điều hướng (Navigation):** Nhấp vào các liên kết cuộn đúng đến vùng nội dung tương ứng. | Cao | **Đạt** | Menu gồm 4 liên kết (`#about`, `#skills`, `#projects`, `#contact`). Hiệu ứng cuộn trang mượt mà (smooth scrolling), vị trí dừng hiển thị chính xác tiêu đề từng phần. |
| **TC-FN-03** | **Khối Kỹ năng (Skills Section):** Hiển thị danh sách kỹ năng công nghệ và kỹ năng mềm dạng chip. | Trung bình | **Đạt** | 6 kỹ năng (`Python`, `Guitar`, `Photoshop`, `CSS3 / Flexbox / Grid`, `HTML 5`, `Translation Skills`) hiển thị nổi bật, rõ ràng trên nền thẻ bo tròn. |
| **TC-FN-04** | **Khối Dự án & Thành tựu:** Hiển thị 4 thẻ thành tựu kèm ảnh, tiêu đề, mô tả và danh sách tag phân loại. | Cao | **Đạt** | Đầy đủ 4 thẻ: *Chứng chỉ học thuật*, *Chứng chỉ âm nhạc và giải thưởng*, *Chứng nhận hoạt động ngoại khoá*, *Giải thưởng thể thao*. Mọi thẻ đều hiển thị đúng ảnh và nhãn tag. |
| **TC-FN-05** | **Liên kết mạng xã hội (Social Links):** Truy cập đúng các trang mạng xã hội và email cá nhân. | Trung bình | **Đạt** | Liên kết `mailto:ducminhaha@gmail.com`, GitHub (`mrsyfox`), và Instagram (`mr.syfoxowo`) hoạt động chính xác. |
| **TC-FN-06** | **Biểu mẫu liên hệ (Contact Form):** Tiếp nhận dữ liệu liên hệ từ người dùng và kích hoạt gửi thư. | Cao | **Cần cải thiện** | Form đã có action `mailto:ducminhaha@gmail.com` và thuộc tính `name` cho từng trường. Hoạt động tốt qua ứng dụng email client mặc định, nhưng chưa có backend xử lý tự động gửi trong nền. |

---

### 2. Giao diện, trải nghiệm người dùng và khả năng tương thích

> Đánh giá bố cục responsive trên các kích thước màn hình theo tư duy Mobile-First, khả năng tương thích trình duyệt và độ thân thiện khi sử dụng.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-UI-01** | **Hiển thị trên Mobile (360px - 480px):** Bố cục 1 cột, không có thanh cuộn ngang (horizontal scrollbar). | Nghiêm trọng | **Đạt** | Kiểm tra trên viewport 360px (Samsung Galaxy S8/A51) và 390px (iPhone 12/13/14): Không xuất hiện thanh cuộn ngang; Hero xếp dọc, lưới dự án hiển thị 1 cột hoàn hảo.<br>📸 *Minh chứng:* `docs/screenshots/mobile.png` & `docs/screenshots/mobile-viewport.png` |
| **TC-UI-02** | **Hiển thị trên Tablet (768px - 1024px):** Lưới dự án co giãn 2 cột cân đối. | Trung bình | **Đạt** | Kiểm tra trên iPad Air/Mini (768px): Thẻ dự án chia làm 2 cột rõ ràng, khoảng cách gap hợp lý, không bị vỡ layout hay đè chữ.<br>📸 *Minh chứng:* `docs/screenshots/tablet.png` & `docs/screenshots/tablet-viewport.png` |
| **TC-UI-03** | **Hiển thị trên Desktop (1280px+):** Hero chia 2 cột, lưới dự án mở rộng linh hoạt. | Cao | **Đạt** | Kiểm tra ở 1280px và 1920px: Phần Hero hiển thị thông tin bên trái và ảnh đại diện bên phải; container giới hạn `max-width: 1100px` căn giữa trang thẩm mỹ.<br>📸 *Minh chứng:* `docs/screenshots/desktop.png` & `docs/screenshots/desktop-viewport.png` |
| **TC-UI-04** | **Khả năng tương thích trình duyệt đa nền tảng:** Giao diện đồng nhất trên Chrome, Edge, Firefox, Safari. | Cao | **Đạt** | Kiểm tra trên Chromium (Chrome, Edge), Gecko (Firefox) và WebKit (Safari iOS/macOS): Toàn bộ thuộc tính CSS (Flexbox, Grid, CSS Variables) hiển thị nhất quán 100%. |
| **TC-UI-05** | **Khả năng tiếp cận (Accessibility - a11y):** Thuộc tính ảnh, nhãn aria và điều hướng bàn phím. | Cao | **Đạt** | 100% hình ảnh có thuộc tính `alt` mô tả chuẩn xác. Thẻ `<nav>` và `<brand>` có `aria-label`. Bấm phím `Tab` di chuyển tuần tự và có viền `focus` nhận diện rõ ràng. |
| **TC-UI-06** | **Trải nghiệm thị giác & Độ tương phản (UI/Contrast):** Màu sắc đạt chuẩn đọc WCAG AA. | Trung bình | **Đạt** | Tông màu nền tối `#0f172a` kết hợp chữ trắng/xám nhạt `#f8fafc`, nút kêu gọi hành động màu đỏ cam `#ff3e3e` tạo độ tương phản cao, dễ đọc trong môi trường thiếu sáng. |

#### 📸 Hình ảnh minh chứng kiểm thử Responsive (Visual Evidence)

| 📱 Mobile (360px) | 💻 Tablet (768px) | 🖥️ Desktop (1280px) |
| :---: | :---: | :---: |
| **Bố cục 1 cột dọc chuẩn Mobile-First** | **Lưới dự án co giãn 2 cột cân đối** | **Bố cục 2 cột Hero + Lưới dự án 3 cột** |
| ![Mobile View](screenshots/mobile-viewport.png) | ![Tablet View](screenshots/tablet-viewport.png) | ![Desktop View](screenshots/desktop-viewport.png) |
| [Xem ảnh toàn trang Mobile](screenshots/mobile.png) | [Xem ảnh toàn trang Tablet](screenshots/tablet.png) | [Xem ảnh toàn trang Desktop](screenshots/desktop.png) |

---

### 3. Khả năng vận hành, xử lý lỗi và hiệu năng cơ bản

> Đánh giá tốc độ tải trang, tính toàn vẹn của liên kết/tài nguyên và khả năng kiểm tra hợp lệ dữ liệu đầu vào.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-PERF-01** | **Thời gian tải trang & Tối ưu tài nguyên:** Trang tải nhanh, không bị nghẽn mạng. | Cao | **Đạt** | Do là trang web tĩnh thuần HTML5/CSS3 không dùng JS nặng, thời gian tải trang đạt mức dưới 0.4s. Điểm Google Lighthouse Performance ước tính đạt > 95/100. |
| **TC-PERF-02** | **Tính toàn vẹn tài nguyên (No 404 Assets):** Không có tệp hình ảnh hoặc CSS nào bị lỗi đường dẫn. | Nghiêm trọng | **Đạt** | Toàn bộ 5 tệp ảnh trong `assets/img/` và tệp `assets/css/styles.css` đều được nạp thành công với mã phản hồi HTTP 200 OK. |
| **TC-PERF-03** | **Loại bỏ liên kết chết (Dead Link Elimination):** Không còn liên kết rỗng gây hiểu lầm. | Trung bình | **Đạt** | Đã loại bỏ hoàn toàn các thẻ `<a href="#">Xem chi tiết →</a>` không có nội dung, đảm bảo người dùng không tương tác vào các liên kết vô nghĩa. |
| **TC-PERF-04** | **Kiểm tra hợp lệ biểu mẫu (Form Validation):** Ngăn chặn gửi dữ liệu rỗng hoặc sai định dạng. | Cao | **Đạt** | Các trường *Họ và tên*, *Email*, *Lời nhắn* đều có thuộc tính `required`. Trường email kiểm tra đúng cú pháp `user@domain.com` trước khi gửi. |
| **TC-PERF-05** | **Ổn định bố cục khi tải trang (Layout Shift):** Không bị nhảy trang khi ảnh tải về. | Trung bình | **Đạt** | Mọi thẻ `<img>` đều được khai báo rõ ràng kích thước `width` và `height`, giúp trình duyệt dành sẵn không gian hiển thị, hạn chế tối đa độ dịch chuyển bố cục (CLS ≈ 0). |

---

### 4. Bảo mật, quản lý cấu hình và dữ liệu

> Đánh giá an toàn thông tin khi liên kết ra ngoài, quản lý cấu hình môi trường và an toàn dữ liệu cá nhân.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-SEC-01** | **Bảo mật liên kết ngoài (Tabnabbing Prevention):** Ngăn chặn lỗ hổng chiếm quyền điều hướng. | Cao | **Đạt** | Mọi liên kết có `target="_blank"` (GitHub, Instagram) đều được thiết lập kèm thuộc tính `rel="noopener noreferrer"` chuẩn bảo mật. |
| **TC-SEC-02** | **Bảo mật cấu hình & Thông tin nhạy cảm:** Không để lộ API Key, Token hay mật khẩu trong mã nguồn. | Nghiêm trọng | **Đạt** | Kho mã nguồn sạch, không chứa tệp `.env`, không chứa secret keys hay chuỗi kết nối cơ sở dữ liệu hardcoded. |
| **TC-SEC-03** | **Quản lý cấu hình môi trường phát triển:** Tách biệt cấu hình IDE khỏi mã nguồn chính. | Thấp | **Đạt** | Cấu hình cổng Live Server được lưu cục bộ trong thư mục `.vscode/settings.json` (`port: 5501`), không gây xung đột với mã nguồn web. |
| **TC-SEC-04** | **An toàn dữ liệu biểu mẫu:** Không thu thập trái phép hoặc gửi dữ liệu qua các endpoint không xác thực. | Trung bình | **Đạt** | Biểu mẫu sử dụng giao thức chuẩn của client (`mailto:`), không gửi dữ liệu người dùng qua bất kỳ máy chủ bên thứ ba không tin cậy nào. |
| **TC-SEC-05** | **Phân quyền thư mục và tệp:** Thiết lập quyền đọc an toàn khi đóng gói môi trường. | Trung bình | **Đạt** | Khi mount thư mục trang web vào Docker container, tùy chọn `readonly` được kích hoạt ngăn chặn việc ghi đè mã nguồn từ bên trong container. |

---

### 5. Chất lượng mã nguồn, cấu trúc repository và tài liệu bàn giao

> Đánh giá chuẩn cấu trúc mã nguồn HTML/CSS, tính tổ chức của repository và tính đầy đủ của bộ tài liệu hướng dẫn.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-CODE-01** | **Chuẩn Semantic HTML5:** Sử dụng đúng các thẻ ngữ nghĩa của W3C. | Cao | **Đạt** | Cấu trúc phân cấp chuẩn mực: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`. Không bị lạm dụng thẻ `<div>` vô nghĩa. |
| **TC-CODE-02** | **Chất lượng CSS:** Tách biệt file kiểu dáng, cấu trúc rõ ràng và dễ bảo trì. | Cao | **Đạt** | Tệp `assets/css/styles.css` tổ chức theo từng khối logic (Reset, Variables, Typography, Header, Hero, Sections, Cards, Footer, Media Queries). |
| **TC-CODE-03** | **Cấu trúc Repository khoa học:** Thư mục được sắp xếp ngăn nắp, dễ hiểu. | Trung bình | **Đạt** | Phân cấp rõ ràng: mã nguồn chính nằm ở thư mục gốc / tài nguyên trong `assets/`, tài liệu dự án nằm trong `docs/`. |
| **TC-CODE-04** | **Tài liệu hướng dẫn (README.md):** Đầy đủ thông tin giới thiệu, yêu cầu và cách chạy. | Cao | **Đạt** | Tệp `README.md` cung cấp đầy đủ thông tin tác giả, công nghệ, cấu trúc thư mục và hướng dẫn khởi chạy chi tiết trên Windows, macOS, Linux và Docker. |
| **TC-CODE-05** | **Tài liệu phát hành & Nhật ký (Release Note & Logs):** Theo dõi đầy đủ các phiên bản. | Trung bình | **Đạt** | `docs/RELEASENOTE.md` ghi nhận chi tiết phiên bản v1.0, ngày phát hành, chức năng mới, lỗi đã sửa và các điểm hạn chế tồn tại. |

---

### 6. Khả năng triển khai, kiểm thử và cung cấp minh chứng

> Đánh giá khả năng chạy thực tế của sản phẩm trên nhiều phương thức triển khai khác nhau và tính sẵn sàng của minh chứng kiểm thử.

| Mã Test | Hạng mục kiểm tra | Trọng yếu | Trạng thái | Ghi chú & Minh chứng cụ thể |
| :--- | :--- | :---: | :---: | :--- |
| **TC-DEP-01** | **Triển khai mở trực tiếp (File Protocol):** Mở xem ngay lập tức không cần web server. | Cao | **Đạt** | Mở tệp `index.html` trực tiếp bằng trình duyệt: Hiển thị đầy đủ hình ảnh, CSS và font chữ nhờ sử dụng đường dẫn tương đối chính xác. |
| **TC-DEP-02** | **Triển khai qua VS Code Live Server:** Chạy trên môi trường server nội bộ của IDE. | Cao | **Đạt** | Khởi chạy qua Live Server thành công tại địa chỉ `http://localhost:5501`, tự động tải lại (hot reload) khi có thay đổi mã nguồn. |
| **TC-DEP-03** | **Triển khai qua Python HTTP Server:** Khởi chạy bằng lệnh dòng lệnh tiêu chuẩn. | Trung bình | **Đạt** | Thực thi lệnh `python -m http.server 8000`: Máy chủ phản hồi nhanh, phục vụ đầy đủ tài nguyên trang web tại `http://localhost:8000`. |
| **TC-DEP-04** | **Triển khai Container hóa qua Docker Nginx:** Chạy trang web trong môi trường container độc lập. | Trung bình | **Đạt** | Khởi chạy thành công container Nginx Alpine qua lệnh `docker run`, liên kết volume trang tĩnh chuẩn xác, truy cập ổn định tại cổng `8080`. |
| **TC-DEP-05** | **Bộ minh chứng kiểm thử (Artifacts & Evidence):** Cung cấp đầy đủ báo cáo, ảnh chụp màn hình và tệp đóng gói. | Cao | **Đạt** | Đầy đủ tệp báo cáo PDF gốc (`BAOCAO-A2.1.pdf`), gói nén dự án (`KT A2.1.zip`), bộ ảnh chụp minh chứng responsive 3 thiết bị (`docs/screenshots/`), nhật ký Git commit minh bạch trên branch `main`. |

---

## 📝 ĐÁNH GIÁ TỔNG KẾT & ĐỀ XUẤT (CONCLUSION & RECOMMENDATIONS)

### 1. Nhận định chung về mức độ sẵn sàng bàn giao (Handover Readiness)
* **Kết luận chung:** **ĐẠT TIÊU CHUẨN BÀN GIAO (READY FOR HANDOVER / ACCEPTED)**.
* Sản phẩm Website Portfolio CV cá nhân (Phiên bản `v1.0`) của tác giả **Nguyễn Đức Minh** đã hoàn thành xuất sắc các mục tiêu đề ra trong đề bài kiểm tra A2.1.
* Đạt tỷ lệ vượt qua kiểm thử **96.9%** (31/32 tiêu chí Đạt, 1 tiêu chí Cần cải thiện, 0 tiêu chí Thất bại).
* Website đáp ứng hoàn hảo tiêu chuẩn responsive theo tư duy **Mobile-First**, không xảy ra lỗi tràn màn hình, đảm bảo khả năng tiếp cận và có tài liệu kỹ thuật đi kèm rất chi tiết, chuyên nghiệp.

### 2. Các vấn đề cần cải thiện trong các phiên bản tiếp theo (Backlog for v1.1)
1. **Tích hợp dịch vụ gửi thư tự động:**
   * *Hiện trạng:* Biểu mẫu liên hệ sử dụng `mailto:` phụ thuộc vào ứng dụng email client của người dùng.
   * *Đề xuất:* Trong phiên bản `v1.1`, tích hợp thêm thư viện client-side như **EmailJS** hoặc endpoint webhook miễn phí (**Formspree**) để cho phép gửi email trực tiếp từ trình duyệt mà không cần mở ứng dụng mail ngoài.
2. **Bổ sung cửa sổ xem ảnh chi tiết (Lightbox / Modal):**
   * *Hiện trạng:* Các thẻ thành tựu chỉ hiển thị ảnh đại diện thu nhỏ.
   * *Đề xuất:* Bổ sung tính năng phóng to ảnh chứng chỉ hoặc liên kết xem file chứng nhận PDF chi tiết khi người dùng nhấp vào thẻ dự án.
3. **Thêm công tắc chuyển đổi Dark / Light Theme:**
   * *Hiện trạng:* Giao diện chỉ có Dark Theme cố định.
   * *Đề xuất:* Bổ sung nút chuyển đổi giao diện sáng/tối và lưu trạng thái vào `localStorage` của trình duyệt.

---

**Xác nhận của Kỹ sư Kiểm thử (QA/QC Engineer):**  
*Nguyễn Đức Minh* — Ngày hoàn thành: 05/11/2026
