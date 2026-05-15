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

 3.1. Admin 

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

| 1   | Tổng quát                     | Admin, Nhân viên |

| 2   | Quản lý tài khoản nhân viên   | Admin            |

| 3   | Tạo công việc mới             | Admin            |

| 4   | Phân công công việc           | Admin            |

| 5   | Theo dõi tiến độ công việc    | Admin            |

| 6   | Quản lý danh sách công việc   | Admin            |

| 7   | Xem công việc được giao       | Nhân viên        |

| 8   | Cập nhật trạng thái công việc | Nhân viên        |

| 9   | Xem báo cáo công việc         | Admin            |


 6. Phân tích Use Case chi tiết

 6.1. Use Case tổng quát

Mục đích

   Mô tả chức năng của hệ thống theo từng người dùng.

Actor

    Admin
    Nhân viên
  
Use Case cần có

Admin

   Đăng nhập hệ thống
   
   Quản lý tài khoản nhân viên

   Tạo công việc mới
   
   Phân công công việc
   
   Theo dõi tiến độ công việc
   
   Quản lý danh sách công việc
   
   Xem báo cáo

Nhân viên

    Đăng nhập hệ thống
    
    Xem danh sách công việc được giao
    
    Cập nhật trạng thái công việc
    
    Báo cáo công việc

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

   → Vào hệ thống
   
   → Sai → Báo lỗi
   
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

Biểu đồ mô tả quá trình xác thực tài khoản của nhân viên trên hệ thống.

     Bước 1: Nhân viên nhập thông tin tài khoản vào giao diện Đăng nhập (Login UI).
     
     Bước 2: Login UI gửi dữ liệu đăng nhập đến Server.
     
     Bước 3: Server gửi yêu cầu kiểm tra thông tin tài khoản xuống Database.
     
     Bước 4: Database trả kết quả xác thực về cho Server.
     
     Bước 5 (Trường hợp đúng): Nếu tài khoản chính xác, Server phản hồi trạng thái "Đúng tài khoản" tới Login UI.
     
     Bước 6: Login UI chuyển hướng và hiển thị trang chủ cho Nhân viên.
     
     Bước 7 (Trường hợp sai): Nếu tài khoản sai, Server phản hồi trạng thái "Sai tài khoản" tới Login UI.
     
     Bước 8: Login UI thông báo lỗi và yêu cầu Nhân viên nhập lại thông tin.

9.2. Sequence Diagram — Tạo công việc

Biểu đồ mô tả quy trình Admin khởi tạo một công việc mới trên hệ thống.

    Bước 1: Admin nhập thông tin công việc mới vào giao diện Task Admin UI.
    
    Bước 2: Giao diện gửi dữ liệu công việc đến Server.
    
    Bước 3: Server yêu cầu Database kiểm tra tính hợp lệ/trùng lặp của dữ liệu.
    
    Bước 4, 5, 6 (Trường hợp trùng): Nếu dữ liệu bị trùng, Database báo về Server, sau đó Server trả thông báo lỗi về UI và yêu cầu Admin nhập lại.
    
    Bước 7, 8, 9: Nếu dữ liệu không trùng, Server gửi yêu cầu xác nhận lưu công việc đến giao diện. Admin thực hiện xác nhận lưu trên màn hình.
    
    Bước 10, 11: Sau khi xác nhận, Task Admin UI gửi yêu cầu lưu chính thức đến Server.
    
    Bước 12, 13: Server thực hiện lệnh lưu công việc vào Database và nhận phản hồi "Lưu thành công".
    
    Bước 14: Server gửi thông báo "OK" (Thành công) hiển thị trên màn hình cho Admin.

9.3. Sequence Diagram — Cập nhật trạng thái công việc

Biểu đồ mô tả quá trình nhân viên thay đổi trạng thái tiến độ của một công việc.

    Bước 1: Nhân viên chọn một công việc cụ thể trên giao diện Task Nhân viên UI.
    
    Bước 2, 3: UI gửi yêu cầu đến Server, sau đó Server truy xuất thông tin công việc từ Database để kiểm tra.
    
    Bước 4, 5: Sau khi xác nhận dữ liệu đúng, Server yêu cầu Nhân viên thực hiện chọn trạng thái mới trên UI.
    
    Bước 6, 7: Nhân viên chọn trạng thái và nhấn cập nhật trên giao diện.
    
    Bước 8, 9: Dữ liệu trạng thái mới được gửi từ UI đến Server và tiếp tục được gửi xuống Database để kiểm tra tính hợp lệ.
    
    Bước 10, 11: Khi Database phản hồi dữ liệu "Hợp lệ", Server gửi tín hiệu cho giao diện để hiển thị trạng thái công việc mới đã được cập nhật thành công.

10. Class Diagram
    
-Class Nhân viên:
ID;
Tên đăng nhập;
Password;
Họ tên;
Vai trò;
Email;
SDT

-Class Công việc:
ID công việc;
Tên công việc;
Mô tả;
Trạng thái;
Hạn hoàn thành;
Ngày tạo;
Người được giao

-Class Thông báo:
ID thông báo;
Nội dung;
Ngày tạo;
Người nhận;
Trạng thái

Quan hệ

Nhân viên 1 --- * Công việc

Nhân viên 1 --- * Thông báo

11. Thiết kế cơ sở dữ liệu sơ bộ
    
-Bảng Nhân viên:

ID;
Tên đăng nhập;
Password;
Họ tên;
Vai trò;
Email;
SDT

-Bảng Công việc:

ID công việc;
Tên công việc;
Mô tả;
Trạng thái;
Hạn hoàn thành;
Ngày tạo;
Người được giao

-Bảng Thông báo:

ID thông báo;
Nội dung;
Ngày tạo;
Người nhận;
Trạng thái
