# Portfolio cá nhân – Nguyễn Đức Minh

Website portfolio/CV cá nhân giới thiệu Nguyễn Đức Minh, các kỹ năng, thành tích và thông tin liên hệ. Đây là dự án web tĩnh, phù hợp để xem trực tiếp trên trình duyệt hoặc phục vụ bằng một web server đơn giản.

## Chức năng

- Giới thiệu cá nhân và định hướng nghề nghiệp.
- Trình bày các kỹ năng dưới dạng thẻ.
- Hiển thị các thành tích, chứng chỉ và hoạt động kèm hình ảnh.
- Điều hướng nhanh đến phần Giới thiệu, Kỹ năng, Dự án và Liên hệ.
- Giao diện responsive cho điện thoại, máy tính bảng và máy tính.
- Cung cấp email, GitHub, Instagram và biểu mẫu liên hệ giao diện.

> **Lưu ý:** Biểu mẫu liên hệ hiện chỉ là giao diện HTML; chưa kết nối dịch vụ gửi email hay máy chủ để xử lý tin nhắn. Các liên kết “Xem chi tiết” trong danh sách thành tích cũng chưa trỏ đến trang nội dung riêng.

## Công nghệ

- HTML5
- CSS3 (Flexbox, CSS Grid, custom properties và media queries)
- Không cần framework, thư viện JavaScript, cơ sở dữ liệu hoặc bước biên dịch.
- Docker tùy chọn: dùng image Nginx để phục vụ trang tĩnh.

## Cấu trúc dự án

```text
profolio/
├── README.md
└── KT A2.1/
    ├── index.html
    ├── assets/
    │   ├── css/
    │   │   └── styles.css
    │   └── img/
    └── .vscode/
        └── settings.json
```

Thư mục trang web cần chạy là `KT A2.1`.

## Yêu cầu môi trường

Để xem trang:

- Trình duyệt hiện đại như Chrome, Firefox, Edge hoặc Safari.
- Không cần cài đặt runtime hay package cho cách mở trực tiếp.

Để chạy bằng máy chủ cục bộ:

- Python 3 (tùy chọn), hoặc Visual Studio Code cùng tiện ích Live Server.

Để chạy bằng Docker:

- Docker Engine trên Linux, hoặc Docker Desktop trên Windows/macOS.
- Docker daemon đang hoạt động.

## Cài đặt

Tải hoặc sao chép dự án về máy, sau đó mở thư mục dự án. Không cần cài thêm dependency.

Nếu dùng Git:

```bash
git clone <URL-kho-ma-nguon>
cd profolio
```

Thay `<URL-kho-ma-nguon>` bằng địa chỉ kho mã nguồn thực tế. Nếu bạn đã có thư mục dự án, bỏ qua bước clone.

## Cấu hình

- Trang chính: `KT A2.1/index.html`.
- Kiểu dáng: `KT A2.1/assets/css/styles.css`.
- Hình ảnh: `KT A2.1/assets/img/`.
- Cổng Live Server được cấu hình là `5501` trong `KT A2.1/.vscode/settings.json`.
- Không có biến môi trường, tệp `.env` hay cấu hình backend cần thiết.

Để thay đổi nội dung, chỉnh sửa HTML; để thay đổi giao diện, chỉnh sửa CSS. Giữ nguyên đường dẫn tương đối đến các tệp trong `assets` để hình ảnh và kiểu dáng tiếp tục được tải đúng.

## Chạy thử

### Windows

**Mở trực tiếp:** Mở `KT A2.1\index.html` bằng trình duyệt.

**Dùng Python:** Mở PowerShell tại thư mục gốc dự án và chạy:

```powershell
cd '.\KT A2.1'
py -m http.server 8000
```

Nếu lệnh `py` không có nhưng Python đã được cài và thêm vào `PATH`, dùng `python -m http.server 8000`.

### macOS

Trong Terminal, từ thư mục gốc dự án:

```bash
cd "KT A2.1"
python3 -m http.server 8000
```

### Linux

Trong terminal, từ thư mục gốc dự án:

```bash
cd "KT A2.1"
python3 -m http.server 8000
```

Sau khi máy chủ khởi động, mở <http://localhost:8000>. Dừng máy chủ bằng `Ctrl+C`.

### Dùng Visual Studio Code Live Server

1. Mở thư mục `KT A2.1` trong Visual Studio Code.
2. Cài tiện ích **Live Server** nếu chưa có.
3. Mở `index.html`, chọn **Go Live**.
4. Truy cập <http://localhost:5501> (cổng đã cấu hình trong workspace).

### Docker

Các lệnh sau gắn thư mục `KT A2.1` vào Nginx, không cần tạo image riêng. Đảm bảo Docker đang chạy và chạy lệnh tại thư mục gốc dự án.

**Windows (PowerShell):**

```powershell
$site = (Resolve-Path '.\KT A2.1').Path
docker run --rm -d --name profolio -p 8080:80 --mount "type=bind,source=$site,target=/usr/share/nginx/html,readonly" nginx:alpine
```

**macOS / Linux (Bash hoặc shell tương thích):**

```bash
docker run --rm -d --name profolio -p 8080:80 \
  --mount "type=bind,source=$(pwd)/KT A2.1,target=/usr/share/nginx/html,readonly" \
  nginx:alpine
```

Mở <http://localhost:8080> để xem trang. Dừng container bằng:

```bash
docker stop profolio
```

## Thông tin liên hệ

- **Email:** [ducminhaha@gmail.com](mailto:ducminhaha@gmail.com)
- **GitHub:** [mrsyfox](https://github.com/mrsyfox)
- **Instagram:** [@mr.syfoxowo](https://www.instagram.com/mr.syfoxowo/)