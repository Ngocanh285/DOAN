# DOAN
### Cách cài đặt:
* Máy đã cài môi trường Node JS
* Clone source từ github
* Mở source trên môi trường code, vd: visual studio code
* Trong Visual Studio Code mở terminal và chia thành 2 tab. Sau đó cd đến 2 thư mục Client và Server. 
* Trong client và server trên có 1 file là env. Tại file env của server là file môi trường chạy có thể sửa đổi cổng, khóa hàm băm của password, trên DB, máy chủ, tên máy chủ, nếu có đặt password của DB thì nhập password DB vào. Bắt buộc: Bổ sung phần cloudinary cho file env của cả client và server, email dùng để gửi mail về cho tài khoản đăng ký bên server.
* Email để gửi mail chắc chắn là email đã xác thực số điện thoại và có 2 bước bảo mật.
* Đầu tiên, tạo tài khoản cloudinary, sau đó đăng nhập vào trang chủ dashboard có thể thấy được thông tin của tài khoản. Copy cloud_name dán vào Cloud_name của file env client và Cloudinary_name của file env server. Copy API key dán vào Cloudinary_key của file env server. Copy API secret dán vào Cloudinary_secret của file env server.
* Tiếp theo, sử dụng 1 email đã xác thực vào mục mật khẩu ứng dụng đặt tên ứng dụng là phòng trọ hoặc bất kỳ và enter. Google sẽ render ra 1 đoạn mã copy mã đó vào phần EMAIL_APP_PASWORD trong file env của server, copy email dán vào EMAIL_NAME.
* Tiếp theo, đấy data lên mysql. Đảm bảo có Xampp, khởi động xampp, mở mysql. Đồng thời ở 2 cửa sổ terminal tại client chạy lệnh npm i --force và tại server chạy lệnh npm i để tải các module về project.
* Trên mysql tạo một cơ sở dữ liệu có tên là phongtro để server đẩy data lên. Vào import chọn file phongtro.sql có sẵn trong project import vào mysql.
* Cuối cùng thì vào terminal npm start server và client.
* Lưu ý khi đăng ký dùng email khác với email gửi vì email gửi không thể gửi được cho chính nó.