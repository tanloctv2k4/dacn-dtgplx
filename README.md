# 🚗 Hệ thống Luyện thi & Quản lý GPLX

> Hệ thống quản lý đào tạo và luyện thi giấy phép lái xe được phát triển bằng **ASP.NET Core MVC**. Ứng dụng hỗ trợ học lý thuyết, thi thử, thi mô phỏng, đăng ký khóa học, thuê xe tập lái, thanh toán trực tuyến và quản lý trung tâm đào tạo.

---

## 📖 Mục lục

- [Giới thiệu](#-giới-thiệu)
- [Tính năng chính](#-tính-năng-chính)
- [Công nghệ sử dụng](#-công-nghệ-sử-dụng)
- [Kiến trúc dự án](#-kiến-trúc-dự-án)
- [Cấu trúc thư mục](#-cấu-trúc-thư-mục)
- [Cài đặt và chạy dự án](#-cài-đặt-và-chạy-dự-án)
- [Thanh toán & Tích hợp](#-thanh-toán--tích-hợp)
- [AI Chatbot & OCR](#-ai-chatbot--ocr)
- [Ảnh minh họa](#-ảnh-minh-họa)
- [Định hướng phát triển](#-định-hướng-phát-triển)
- [Tác giả](#-tác-giả)

---

# 📌 Giới thiệu

Hệ thống được xây dựng nhằm hỗ trợ các trung tâm đào tạo lái xe trong việc quản lý học viên, giáo viên, khóa học và quá trình đào tạo. Đồng thời cung cấp nền tảng học tập trực tuyến giúp học viên ôn tập lý thuyết, thi thử, thi mô phỏng và theo dõi kết quả học tập.

---

# ✨ Tính năng chính

## 👨‍🎓 Học viên

- Đăng ký, đăng nhập
- Đăng nhập bằng Google và Facebook
- Ôn tập lý thuyết theo từng chương
- Học câu điểm liệt
- Học biển báo giao thông bằng Flashcard
- Thi thử lý thuyết
- Thi mô phỏng tình huống giao thông
- Xem lịch học
- Đăng ký khóa học
- Thuê xe tập lái
- Thanh toán trực tuyến
- Chat với giáo viên
- Chatbot AI hỗ trợ giải đáp
- Nhận thông báo từ hệ thống

---

## 👨‍🏫 Giáo viên

- Quản lý lịch dạy
- Theo dõi học viên
- Quản lý lớp học
- Trao đổi với học viên

---

## 👨‍💼 Quản trị viên

- Dashboard thống kê
- Quản lý tài khoản
- Quản lý học viên
- Quản lý giáo viên
- Quản lý khóa học
- Quản lý lịch học
- Quản lý đề thi
- Quản lý câu hỏi
- Quản lý bài thi
- Quản lý biển báo
- Quản lý Flashcard
- Quản lý xe tập lái
- Quản lý hóa đơn
- Quản lý thanh toán
- Quản lý phản hồi
- Gửi thông báo
- Báo cáo thống kê

---

# 🛠 Công nghệ sử dụng

| Công nghệ | Mô tả |
|-----------|------|
| ASP.NET Core MVC | Framework phát triển ứng dụng |
| Entity Framework Core | ORM |
| SQL Server | Hệ quản trị cơ sở dữ liệu |
| Razor View | Giao diện |
| Bootstrap 5 | Responsive UI |
| JavaScript / jQuery | Frontend |
| SignalR | Chat thời gian thực |
| JWT Authentication | Xác thực API |
| BCrypt | Mã hóa mật khẩu |
| Swagger | API Documentation |
| MailKit | Gửi Email |
| VNPay | Thanh toán |
| PayPal | Thanh toán |
| MoMo | Thanh toán |
| OpenAI API | AI Chatbot |
| Python OCR | Nhận diện văn bản |

---

# 🏗 Kiến trúc dự án

```
Presentation Layer
        │
ASP.NET Core MVC
        │
Business Services
        │
Entity Framework Core
        │
SQL Server
```

---

# 📂 Cấu trúc thư mục

```
dacn-dtgplx
│
├── Controllers
├── Models
├── ViewModels
├── DTOs
├── Services
├── Helpers
├── Hubs
├── Views
├── wwwroot
├── PythonScripts
├── Data
├── appsettings.json
├── Program.cs
└── README.md
```

---

# ⚙️ Cài đặt và chạy dự án

## 1. Clone project

```bash
git clone https://github.com/yourusername/dacn-dtgplx.git
```

## 2. Di chuyển vào thư mục

```bash
cd dacn-dtgplx
```

## 3. Khôi phục package

```bash
dotnet restore
```

## 4. Cấu hình Database

Cập nhật chuỗi kết nối trong

```
appsettings.json
```

Ví dụ:

```json
"ConnectionStrings": {
    "DefaultConnection": "Server=.;Database=DtGPLX;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

## 5. Chạy dự án

```bash
dotnet run
```

---

# 💳 Thanh toán & Tích hợp

Hệ thống hỗ trợ nhiều phương thức thanh toán:

- VNPay
- PayPal
- MoMo

Ngoài ra còn tích hợp:

- Google Login
- Facebook Login
- MailKit
- SignalR
- QR Code

---

# 🤖 AI Chatbot & OCR

Hệ thống tích hợp AI hỗ trợ:

- Trả lời câu hỏi liên quan GPLX
- Tìm kiếm thông minh
- OCR nhận diện văn bản
- Semantic Search bằng Embedding

---



# 🚀 Định hướng phát triển

- Mobile App
- AI đánh giá kết quả học tập
- Thông báo thời gian thực
- Dashboard nâng cao
- Docker Deployment
- CI/CD Pipeline
- Azure/AWS Deployment

---

# 👨‍💻 Tác giả

**Nguyễn Tấn Lộc**

Sinh viên ngành **Hệ thống Thông tin**

### Kỹ năng

- ASP.NET Core MVC
- C#
- SQL Server
- Entity Framework Core
- RESTful API
- Git & GitHub
- Postman
- Business Analysis
- Software Testing

---

## ⭐ Nếu dự án hữu ích

Hãy để lại một ⭐ cho repository nếu bạn thấy dự án hữu ích.

---
