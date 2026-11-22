# AI Log - Website Portfolio CV Cá Nhân

## 1. Thông tin chung

| Mục | Thông tin |
| :--- | :--- |
| Tên dự án | Website Portfolio CV cá nhân - Nguyễn Đức Minh |
| Phiên bản tài liệu | v1.0 |
| Ngày ghi nhật ký | 23/11/2026 |
| Công cụ AI | GitHub Copilot sử dụng Copilot SDK trong VS Code |
| Vai trò của AI | Phân tích dự án, đề xuất chỉnh sửa, tạo tài liệu và hỗ trợ kiểm tra |
| Quy trình phê duyệt | Nội dung do AI đề xuất hoặc tạo; tác giả dự án kiểm tra và quyết định nội dung được lưu vào repository |

---

## 2. Phạm vi sử dụng AI

AI được sử dụng để hỗ trợ các công việc sau:

- Rà soát cấu trúc website, tài liệu README, release notes và báo cáo kiểm thử.
- Hỗ trợ viết, tổ chức và hoàn thiện tài liệu dự án bằng Markdown.
- Phân tích các phần HTML/CSS đã có trong dự án.
- Kiểm tra tính nhất quán giữa mã nguồn, tài liệu và trạng thái repository.
- Tóm tắt thay đổi, kết quả kiểm tra và các hạn chế còn tồn tại.

AI không thay thế việc kiểm thử giao diện trực tiếp, không giả định kết quả kiểm thử chưa được thực hiện và không thay thế quyết định cuối cùng của tác giả.

---

## 3. Nhật ký phiên làm việc

### Phiên 2026-11-23

| Trường | Nội dung |
| :--- | :--- |
| Công cụ | GitHub Copilot SDK trong VS Code |
| Yêu cầu của người dùng | Viết file `docs/AI_LOG.md` dựa trên dự án |
| Tài liệu được xem | `README.md`, `index.html`, `assets/css/styles.css`, `docs/RELEASENOTE.md`, `docs/test_report.md`, `.vscode/settings.json` |
| Công việc thực hiện | Rà soát công nghệ, chức năng, cấu trúc thư mục, nội dung kiểm thử và lịch sử commit gần nhất |
| Kết quả | Tạo nhật ký AI bằng tiếng Việt, có nguồn gốc dự án và phân biệt rõ thông tin thực tế với phần cần xác minh |
| Trạng thái | Hoàn thành; cần tác giả dự án xem lại và phê duyệt |

#### Prompt chính

- “Viết file ai log dựa trên dự án”
- “Viết file `docs/AI_LOG.md`”

#### Đầu ra của AI

- Tạo tài liệu nhật ký tại `docs/AI_LOG.md`.
- Ghi lại mục đích, phạm vi và quy trình sử dụng AI.
- Ghi nhận các công nghệ và chức năng thực tế của dự án.
- Ghi lại các hạn chế đã được mô tả trong README và tài liệu phát hành.

#### Kiểm tra sau khi tạo

- File AI log nằm đúng thư mục `docs/`.
- Nội dung khớp với tên dự án, tên tác giả, công nghệ và tài liệu hiện có.
- Không thêm thông tin bí mật, khóa API, chuỗi kết nối hoặc dữ liệu cá nhân ngoài những thông tin công khai trong dự án.
- Cần kiểm tra lại cách trình bày nếu repository áp dụng biểu mẫu AI log khác.

---

## 4. Các mốc phát triển có hỗ trợ AI được ghi nhận

Các mục dưới đây được suy ra từ nội dung và lịch sử repository hiện tại. Với các mốc không có git diff hoặc file log riêng, đây là ghi nhận tổng quát chứ không phải bằng chứng đầy đủ cho từng prompt.

| Mốc | Bối cảnh quan sát được | Hỗ trợ dự kiến từ AI | Minh chứng trong dự án |
| :--- | :--- | :--- | :--- |
| Tạo portfolio HTML/CSS | Website giới thiệu cá nhân, kỹ năng, thành tựu và liên hệ | Hỗ trợ thiết kế cấu trúc HTML, phân chia nội dung và viết CSS theo Mobile-First | `index.html`, `assets/css/styles.css` |
| Chuẩn hóa nội dung | Thay đổi tên tác giả, vai trò và mô tả công việc | Hỗ trợ rà soát từ ngữ và cập nhật văn bản nhất quán | Metadata, tiêu đề và phần giới thiệu trong `index.html` |
| Hoàn thiện điều hướng và bố cục | Header cố định, menu anchor, hero 2 cột ở màn hình lớn | Hỗ trợ tách layout theo Flexbox, CSS Grid và media queries | `assets/css/styles.css` |
| Cải thiện khả năng tiếp cận | Thêm `alt`, `aria-label`, `focus-visible` và giảm chuyển động | Hỗ trợ đề xuất thuộc tính ngữ nghĩa và responsive | `index.html`, `assets/css/styles.css` |
| Xây dựng tài liệu bàn giao | README, release notes và test report | Hỗ trợ tổ chức hướng dẫn chạy, danh sách chức năng, lỗi đã sửa và báo cáo kiểm thử | `README.md`, `docs/RELEASENOTE.md`, `docs/test_report.md` |
| Rà soát version | Repository có commit initial và các commit cập nhật animation, smooth transition | Hỗ trợ tóm tắt thay đổi dựa trên mã nguồn và tài liệu | Lịch sử Git của repository |

---

## 5. Prompt và tình huống tiêu biểu

### Prompt: Xây dựng giao diện responsive

**Mục tiêu:**
- Dùng HTML5/CSS3 thuần.
- Hỗ trợ bố cục 1 cột trên mobile, 2 cột trên tablet và 3 cột trên desktop.
- Không làm tràn thanh cuộn ngang.

**Kết quả được áp dụng:**
- CSS Grid cho danh sách thẻ thành tựu.
- Flexbox cho header, thanh điều hướng và danh sách kỹ năng.
- Media queries tại breakpoint 768px và 1280px.

**Cách xác minh:**
- So sánh cấu trúc CSS với các viewport trong `docs/test_report.md`.
- Xem ảnh minh chứng trong `docs/screenshots/`.

### Prompt: Hoàn thiện biểu mẫu liên hệ

**Mục tiêu:**
- Giữ biểu mẫu mà không yêu cầu backend.
- Cho người dùng nhập họ tên, email và lời nhắn.
- Tạo dữ liệu gửi qua email client mặc định.

**Kết quả được áp dụng:**
- Thuộc tính `required` cho các trường bắt buộc.
- Định dạng input `type="email"`.
- Form dùng `action="mailto:"`, `method="post"` và `enctype="text/plain"`.
- Tên trường `name` được đặt cho dữ liệu biểu mẫu.

**Hạn chế đã ghi nhận:**
- Biểu mẫu phụ thuộc vào ứng dụng email client trên máy người dùng.
- Chưa có backend hoặc dịch vụ gửi thư tự động.

### Prompt: Viết tài liệu dự án

**Mục tiêu:**
- Giải thích cách chạy trang trên trình duyệt, Live Server, Python HTTP Server và Docker.
- Ghi nhận chức năng, lỗi đã sửa và giới hạn đã biết.

**Kết quả được áp dụng:**
- `README.md` mô tả cài đặt và các phương thức chạy.
- `docs/RELEASENOTE.md` ghi lại chức năng, bug fixes và hạn chế.
- `docs/test_report.md` ghi lại kết quả kiểm thử theo từng nhóm.

---

## 6. Tác động của AI đến repository

### Thay đổi tích cực

- Giúp thống nhất cấu trúc tài liệu giữa README, release notes và test report.
- Giúp phát hiện các tiêu chí cần kiểm tra về responsive, bố cục, bảo mật liên kết và biểu mẫu.
- Giảm công sức viết tài liệu lặp lại và hỗ trợ tổ chức thông tin theo từng nhóm.
- Giúp ghi nhận hạn chế thay vì che giấu hoặc mô tả các chức năng chưa tồn tại.

### Rủi ro và kiểm soát

- Nội dung do AI đề xuất có thể không khớp hoàn toàn với kết quả kiểm thử thực tế.
- AI có thể suy ra hoặc diễn đạt quá mạnh các kết quả chưa được đo trực tiếp.
- Chỉ các thay đổi đã được kiểm tra và được tác giả chấp nhận mới được đưa vào repository.
- Các cảnh báo, hạn chế và trạng thái “cần cải thiện” phải được kiểm tra lại trước khi bàn giao.

---

## 7. Quy trình kiểm duyệt khuyến nghị

1. Tác giả kiểm tra lại nội dung do AI tạo hoặc chỉnh sửa.
2. Chạy website bằng trình duyệt hoặc Live Server.
3. Kiểm tra các liên kết, hình ảnh, biểu mẫu và responsive tại các viewport đã nêu.
4. Chạy lại báo cáo kiểm thử nếu có thay đổi mã nguồn.
5. Cập nhật release notes và AI log khi phát hành phiên bản mới.
6. Không ghi commit hoặc secret thật vào tài liệu AI log.

---

## 8. Hạn chế còn tồn tại

Theo [README.md](../README.md) và [release notes](RELEASENOTE.md), dự án còn các hạn chế sau:

- Biểu mẫu liên hệ chỉ dùng `mailto:` và phụ thuộc ứng dụng email của người dùng.
- Chưa có trang chi tiết cho từng chứng chỉ hoặc dự án.
- Chưa tích hợp chế độ sáng/tối.
- Chưa có JavaScript cho kiểm tra biểu mẫu thời gian thực hoặc menu đóng/mở trên thiết bị di động.
- Chưa hỗ trợ chuyển đổi Việt/Anh.

Các hạn chế này đã được ghi nhận trong tài liệu thay vì mô tả thành tính năng hoàn chỉnh.

---

## 9. Lịch sử AI log

| Ngày | Phiên bản | Nội dung |
| :--- | :--- | :--- |
| 23/11/2026 | v1.0 | Tạo lần đầu AI log dựa trên cấu trúc, chức năng và tài liệu của dự án |

---

**Người phát hành:** Nguyễn Đức Minh

**Công cụ hỗ trợ:** GitHub Copilot SDK trong VS Code

**Trạng thái:** Tài liệu khởi tạo và chờ kiểm duyệt