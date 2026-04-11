# 🛒 JewelryShop-Springboot 

Dự án **JewelryShop** là một ứng dụng web thương mại điện tử mini được xây dựng bằng  
**Spring boot + Thymeleaf+ Bootstrap + JPA + SQLServer/MySQL/ postgreSQL  +Decorator Sitemesh+ JWT**,  
triển khai theo mô hình **MVC + DAO + Service Layer**.

🎯 **Mục tiêu:** Xây dựng nền tảng mua hàng và quản lý thương mại điện tử mini chuyên về các sản phẩm công nghệ.

---

## 1️⃣ Cấu trúc dự án

```text
Uteshop-servlet/
├── .git/
├── pom.xml               # Quản lý dependencies 
├── src/
│   └── main/
│       ├── java/ute/shop/
│       │   ├── config/                      # Cấu hình kết nối DB, Security, tải dữ liệu ban đầu, và tích hợp thanh toán (Momo, VNPay)
│       │   ├── controller/                  # Xử lý request
│       │   ├── repository/                  # Interface DAO
│       │   ├── entity/                      # Chứa các lớp mô hình dữ liệu
│       │   ├── service/                     # Interface Service
│       │   ├── service/impl/                # Business logic
│       │   ├── service/specification/       # Xử lý tiêu chí lọc & chuyển đổi dữ liệu đầu vào để query database (JPA Specification)
│       │   └──  dto/                        # Các lớp trung gian (Data Transfer Object) dùng cho xác thực, response, hoặc truyền dữ liệu giữa tầng
│       ├── resources/
│       │   ├── fonts/                              # Lưu trữ các font chữ được sử dụng trong giao diện (ví dụ: Roboto, Montserrat)
│       │   ├── static/                             # Các tài nguyên tĩnh: CSS, JS, hình ảnh, icon,...
│       │   ├── templates/                          # Giao diện hiển thị (Thymeleaf Templates)
│       │   │   ├── admin/                          # Giao diện quản trị hệ thống
│       │   │   │   ├── audits/                     # Nhật ký hoạt động của Admin
│       │   │   │   ├── collections/                # Quản lý bộ sưu tập sản phẩm
│       │   │   │   ├── layout/                     # Layout tổng thể cho trang admin
│       │   │   │   ├── orders/                     # Quản lý đơn hàng
│       │   │   │   ├── products/                   # Quản lý sản phẩm
│       │   │   │   ├── shippers/                   # Quản lý đơn vị vận chuyển
│       │   │   │   ├── stocks/                     # Quản lý kho hàng
│       │   │   │   ├── suppliers/                  # Quản lý nhà cung cấp
│       │   │   │   ├── users/                      # Quản lý người dùng
│       │   │   │   └── dashboard.html              # Trang tổng quan cho admin
│       │   │   ├── manager/                        # Giao diện dành cho quản lý (Manager)
│       │   │   │   ├── collections/                # Quản lý bộ sưu tập sản phẩm
│       │   │   │   ├── layout/                     # Layout cho giao diện manager
│       │   │   │   ├── orders/                     # Theo dõi đơn hàng
│       │   │   │   ├── products/                   # Quản lý sản phẩm cửa hàng
│       │   │   │   ├── shippers/                   # Theo dõi tình trạng vận chuyển
│       │   │   │   ├── stocks/                     # Theo dõi tồn kho
│       │   │   │   ├── suppliers/                  # Làm việc với nhà cung cấp
│       │   │   │   └── dashboard.html              # Trang tổng quan dành cho manager
│       │   │   ├── client_1/                       # Giao diện người dùng (client)
│       │   │   │   ├── homepage/                   # Trang chủ và các phần giới thiệu
│       │   │   │   └── layout/                     # Layout tổng thể cho người dùng
│       │   │   └── product/                        # Trang chi tiết sản phẩm
│       │   ├── application.properties              # Cấu hình mặc định (chung cho toàn dự án)
│       │   ├── application-dev.properties          # Cấu hình môi trường phát triển (DEV)
│       │   └── application-prod.properties         # Cấu hình môi trường triển khai (PRODUCTION)
```
## 2️⃣ Các bước cài đặt
1. Cài **MYSQL Server** (tham khảo hướng dẫn trên YouTube)
2. Tạo database **jewelry**
3. Tải mã nguồn **JewelryShop** từ GitHub nhóm
4. Khởi động **Springboot** → truy cập [http://localhost:8080/]
5. Đăng nhập tài khoản **Admin** mặc định:
    - Username: **admin@gmail.com**
    - Password: **admin123**
> Dự án được phát triển theo mô hình phân lớp chuẩn (**MVC – DAO – Service**), đảm bảo dễ bảo trì, mở rộng, và áp dụng các công nghệ hiện đại trong Java Web như **JPA** cùng giao diện thân thiện và hệ thống bảo mật an toàn.

