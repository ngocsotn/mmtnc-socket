# ĐỒ ÁN MMT NC - SOCKET

## Thành viên
- Nguyễn Thế Ngọc
- Vương Gia Huy
- Nguyễn Thị Thúy Hằng
- Lê Nguyễn Trung Kiên

## Yêu cầu
- Có các File server, Server chính và các client.
- Khi File server khởi động, kết nối với Master server và gửi thông tin file. Service 1 dùng giao thức TCP để truyền danh sách, thông tin file server đến Master server.
- Service 2 dùng giao thức TCP giao tiếp giữa Client và Master Server, khi Client cần danh sách file từ toàn bộ file Server thì sẽ gửi tín hiệu đến Master Server, Master Server nhận tín hiệu sẽ gửi danh sách cho Client, Client hiển thị lên danh sách file, thông tin của các File Server.
- Service 3 dùng giao thức UDP. Client tải file về từ file service, có thể tải từ nhiều File Server khác nhau. Mỗi file sẽ có 1 mã MD5, khi tải từng gói tin sẽ kiểm tra MD5 từng gói, nếu đủ gói tin thì hoàn tất, không đủ phải gửi lại gói tin, tránh mất gói tin.
- Công nghệ sử dụng:
    - Ngôn ngữ lập trình C#.
    - Yêu cầu để chạy được bản release là phải có framework .NET 5.0
    - IDE nhóm sử dụng là Visual Studio 2019
    - Master Server và File Server là Console Application, Client là WPF Application.