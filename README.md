# Chào mừng đến với Django

## 1. Front-end và back-end
**Front-end**: là các file HTML, CSS, JS, ... dùng để hiển thị lên phía máy tính người dùng.

**Back-end**: là hệ thống server, dùng để xử lý các *logic của trang web* và chứa đựng *cơ sở dữ liệu*. Công việc chính của lập trình back-end chính là **lập trình server**.

**Cơ sở dữ liệu**: là kho lưu trữ thông tin, sẽ học kỹ hơn ở phần sau.

## 2. Django

**Django** là một thư viện Python (tập hợp những hàm và file viết sẵn, đến khi muốn dùng thì chỉ việc gọi ra mà không cần viết lại). Django cho phép chúng ta lập trình *back-end* nhanh chóng và hiệu quả hơn.

Trong buổi học này, chúng ta sẽ thực hành các bước sau:
- Khởi tạo môi trường ảo với Python. Sử dụng `py -m venv myworld` để khởi tạo môi trường ảo. Sau đó chạy môi trường ảo bằng `myworld\Scripts\activate.bat`.
- Cài đặt Django, sử dụng câu lệnh `pip install Django`. Để kiểm tra xem chúng ta đã cài đặt xong chưa, ta chạy lệnh `django-admin --version`.
- Khởi tạo project mới trong Django sử dụng câu lệnh `django-admin startproject <ten_du_an>`. Sau đó truy cập vào project bằng lệnh `cd <ten_du_an>`.
- Chạy server để thử xem là back-end đã hoạt động chưa bằng lệnh `py manage.py runserver`.
- Khởi tạo app mới bằng `py manage.py startapp <ten_app>`. Sau đó, đăng kí app mới tạo vào trong server bằng cách truy cập đến project, tìm file `settings.py`, tìm đến `INSTALLED_APPS` và thêm tên app của chúng ta vào.
- Tất cả file HTML của một app thì được chứa ở trong thư mục `templates`. Ban đầu, tất cả các app sẽ không có thư mực templates nên chúng ta phải tự tạo ra.
> **Cách tạo folder templates**
>
> Ở trong app của chúng ta, tạo folder như sau `templates/<ten_app>`. Sau đó toàn bộ các file HTML của app đều được đặt trong `templates/<ten_app>`.
- Cài đặt `views.py` và `urls.py` ở app và ở project. *Tự tìm hiểu thêm*.