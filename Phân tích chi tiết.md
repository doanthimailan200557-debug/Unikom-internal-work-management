# PHÂN TÍCH HỆ THỐNG QUẢN LÝ CÔNG VIỆC NỘI BỘ CHO CÔNG TY UNIKOM

 1. Giới thiệu đề tài

Đề tài “Xây dựng hệ thống quản lý công việc nội bộ cho công ty Unikom” được thực hiện nhằm xây dựng một hệ thống web hỗ trợ quản lý công việc cơ bản cho doanh nghiệp. Hệ thống giúp:
- Quản lý tạo công việc
- Phân công công việc cho nhân viên
- Theo dõi tiến độ thực hiện
- Quản lý danh sách công việc nội bộ

 2. Mục tiêu hệ thống

- Xây dựng hệ thống quản lý công việc nội bộ trên nền tảng web
- Hỗ trợ quản lý phân công công việc cho nhân viên
- Theo dõi tiến độ và trạng thái công việc
- Quản lý tài khoản nhân viên
- Hỗ trợ nhân viên cập nhật tiến độ làm việc

 3. Đối tượng sử dụng hệ thống

 3.1. Admin / Quản lý

Admin là người có quyền quản lý toàn bộ hệ thống:
- Quản lý tài khoản nhân viên
- Tạo công việc mới
- Phân công công việc
- Theo dõi tiến độ công việc
- Quản lý danh sách công việc
- Xem báo cáo của nhân viên

 3.2. Nhân viên

Nhân viên sử dụng hệ thống để:
- Đăng nhập hệ thống
- Xem danh sách công việc được giao
- Cập nhật trạng thái công việc
- Báo cáo công việc

 4. Chức năng hệ thống

 4.1. Chức năng dành cho Admin

 Đăng nhập hệ thống
- Đăng nhập bằng tài khoản quản trị
- Kiểm tra quyền truy cập

 Quản lý tài khoản nhân viên
- Thêm tài khoản
- Sửa thông tin
- Xóa tài khoản

 Tạo công việc mới
- Nhập tên công việc
- Nhập mô tả công việc
- Thiết lập deadline

 Phân công công việc
- Chọn nhân viên
- Giao nhiệm vụ
- Theo dõi trạng thái xử lý

 Theo dõi tiến độ công việc
- Theo dõi công việc đang thực hiện
- Theo dõi công việc hoàn thành
- Theo dõi công việc quá hạn

 Quản lý danh sách công việc
- Xem danh sách công việc
- Chỉnh sửa công việc
- Xóa công việc

 4.2. Chức năng dành cho Nhân viên

 Đăng nhập hệ thống
- Đăng nhập bằng tài khoản được cấp

 Xem danh sách công việc được giao
- Xem tên công việc
- Xem trạng thái công việc
- Xem deadline

 Cập nhật trạng thái công việc
- Chưa thực hiện
- Đang thực hiện
- Hoàn thành

Báo cáo công việc
- Báo cáo tiến độ cá nhân
- Báo cáo số lượng công việc hoàn thành

 5. Phân tích Use Case

 5.1. Danh sách Use Case

| STT |       Use Case                | Actor            |
| 1   | Đăng nhập hệ thống            | Admin, Nhân viên |
| 2   | Quản lý tài khoản nhân viên   | Admin            |
| 3   | Tạo công việc mới             | Admin            |
| 4   | Phân công công việc           | Admin            |
| 5   | Theo dõi tiến độ công việc    | Admin            |
| 6   | Quản lý danh sách công việc   | Admin            |
| 7   | Xem công việc được giao       | Nhân viên        |
| 8   | Cập nhật trạng thái công việc | Nhân viên        |
| 9   | Xem báo cáo công việc         | Admin            |


 6. Phân tích Use Case chi tiết

 6.1. Use Case: Đăng nhập hệ thống

 Actor
- Admin
- Nhân viên

 Mô tả
Người dùng đăng nhập vào hệ thống bằng tài khoản được cấp.

 6.2. Use Case: Tạo công việc mới

 Actor
- Admin

 Mô tả
Admin tạo công việc mới trong hệ thống.

 6.3. Use Case: Phân công công việc

 Actor
- Admin

 Mô tả
Admin giao công việc cho nhân viên.


 6.4. Use Case: Cập nhật trạng thái công việc

 Actor
- Nhân viên

 Mô tả
Nhân viên cập nhật tiến độ công việc.

 6.5. Use Case: Theo dõi tiến độ công việc

 Actor
- Admin

 Mô tả
Admin theo dõi tiến độ công việc của nhân viên.

 7. Use Case Diagram

 Actor của hệ thống

 Admin
- Đăng nhập hệ thống
- Quản lý tài khoản nhân viên
- Tạo công việc mới
- Phân công công việc
- Theo dõi tiến độ công việc
- Quản lý danh sách công việc

 Nhân viên
- Đăng nhập hệ thống
- Xem công việc được giao
- Cập nhật trạng thái công việc
- Xem báo cáo công việc


 8. Activity Diagram

 8.1. Activity Diagram — Đăng nhập
Bắt đầu
→ Nhập tài khoản/mật khẩu
→ Kiểm tra dữ liệu
→ Đúng?
   → Có → Vào hệ thống
   → Không → Báo lỗi
→ Kết thúc

8.2. Activity Diagram — Phân công công việc
Bắt đầu
→ Admin tạo công việc
→ Nhập thông tin
→ Chọn nhân viên
→ Lưu dữ liệu
→ Gửi công việc
→ Kết thúc

8.3. Activity Diagram — Cập nhật trạng thái công việc
Bắt đầu
→ Nhân viên chọn công việc
→ Chọn trạng thái
→ Cập nhật dữ liệu
→ Hiển thị trạng thái mới
→ Kết thúc

9. Sequence Diagram
    
9.1. Sequence Diagram — Đăng nhập

User → Login Page: nhập tài khoản
Login Page → Server: gửi dữ liệu
Server → Database: kiểm tra tài khoản
Database → Server: trả kết quả
Server → Login Page: đăng nhập thành công/thất bại

9.2. Sequence Diagram — Tạo công việc

Admin → Task Page: nhập công việc
Task Page → Server: gửi dữ liệu
Server → Database: lưu công việc
Database → Server: xác nhận
Server → Task Page: thông báo thành công

9.3. Sequence Diagram — Cập nhật trạng thái công việc

Nhân viên → Task Page: cập nhật trạng thái
Task Page → Server: gửi trạng thái
Server → Database: cập nhật dữ liệu
Database → Server: xác nhận
Server → Task Page: hiển thị trạng thái mới

10. Class Diagram
    
-Class User
id
username
password
full_name
role 

-Class Task
id
title
description
status
deadline
assigned_to

-Class Notification
id
content
user_id
created_at

Quan hệ
User 1 --- * Task
User 1 --- * Notification

11. Thiết kế cơ sở dữ liệu sơ bộ
    
-Bảng users
id
username
password
full_name
role

-Bảng tasks
id
title
description
status
deadline
assigned_to

-Bảng notifications
id
content
user_id
created_at
