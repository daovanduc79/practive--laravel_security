[Thực hành] Sử dụng Laravel Security
Mục tiêu
Hiểu và thực hiện security dựa trên vai trò trong ứng dụng laravel.

Mô tả 
 Trong phần này, chúng ta sẽ tích hợp Laravel Security vào trong một ứng dụng Laravel MVC. Ứng dụng sẽ có một form để đăng nhập, link để đăng xuất.

Các tài nguyên của hệ thống được được cấu hình cấp quyền truy cập phù hợp cho các đối tượng đã đăng nhập và chưa đăng nhập.

Hướng dẫn
Bước 1: Tạo mới project Laravel với tên Laravel-Security:

Mở Terminal và sử dụng câu lệnh bên dưới để tạo mới project:

composer create-project --prefer-dist laravel/laravel Laravel-Security
Tại terminal sử dụng câu lệnh: php artisan serve để khởi chạy project, mở trình duyệt gõ localhost:8000 để chạy project.

Bước 2:  Tạo một database cho ứng dụng và cấu hình file .env để kết nối đến database vừa tạo.

Bước 3:  Chạy lệnh "php artisan make:auth" để Laravel tự động sinh ra các view, route, controller cần thiết cho chức năng login, logout.

Chạy lệnh "php artisan migrate" để tạo các bảng users, password_resets

Các view sẽ tự sinh trong thư mục: resource/views/auth.

Các controller sẽ tự động sinh ra trong thư mục: app/Http/Controller/Auth

Sử dụng lệnh "php artisan route:list" trên terminal để hiển thị các route.

Bước 4: Ở bước trên chúng ta đã hoàn thiện việc cài đặt, cấu hình chức năng authentication của Laravel. Bước này chúng ta sẽ chạy thử.

Ở giao diện màn hình chủ sẽ có menu Login và Register.

Đầu tiên cần tạo một tài khoản: Bấm vào Register và tạo một tài khoản.

Bước 5:  Sau khi đăng ký người dùng thành công, sẽ tự động đăng nhập, tại đây trên thanh menu sẽ có chức năng Logout.

Mã nguồn tham khảo: https://github.com/codegym-vn/laravel-security.git

Tổng kết:
Qua bài này chúng ta đã thực hành sử dụng Laravel Authentication.
