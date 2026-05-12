# Môn: Phát triển ứng dụng với mã nguồn mở-TEE0421
Lớp: 58KTPM
**Bài tập 03:**  
# SỬ DỤNG WORDPRESS ĐỂ TẠO WEB SITE
## deadline : 23h59 ngày 12 tháng 5 năm 2026.  
1. SỬ DỤNG DOCKER TRÊN UBUNTU ĐỂ TẠO docker ccompose chứa: 
- Mariadb: sử dụng **image: mariadb:latest** để làm hệ quản trị csdl cho wordpress
- Phpmyadmin: sư dụng **image: phpmyadmin:latest** để đăng nhập vào mariadb rồi tạo csdl trống (chỉ để xem, ko cần tạo bảng từ đây, wordpress sẽ làm hết)
- WordPress: Sử dụng **image: wordpress:latest**, truyền các tham số môi trường cho wordpress là các thông tin truy cập csdl mariadb, tạo bởi Phpmyadmin
2. Yêu cầu: sau khi có 3 service này trong file docker-compose.yml :
- Cấu hình để hệ thống chạy
- Sử dụng cloudflare tunnel để public web này lên 1 sub-domain
- Tạo 1 bài viết trong wordpress giới thiệu về bản thân sinh viên: thông tin cá nhân, sở thích, ... bài viết có thể chứa hình ảnh, âm thanh, video, ...
- Tạo 1 bài viết trong wordpress giới thiệu về ngành học mà em yêu thích trong trường TNUT. bài viết phải chứa hình ảnh, video, ...
- Nhận xét việc sử dụng mã nguồn mở wordpress để tạo website (tốn công sức thế nào, dễ/khó dùng ra sao, tốn kém tài nguyên(ssh/ram) của máy chủ ra sao,....)

# BÀI LÀM

1. Tạo thư mục project
   
<img width="392" height="24" alt="{817424EA-5D0D-4DF8-804C-00F67ED65FF8}" src="https://github.com/user-attachments/assets/aeb326f9-8e38-43f9-9ee2-3c28955e17d4" />

2. Tạo file docker-compose.yml

<img width="414" height="25" alt="{6171F1FD-9431-4E41-AAD9-99F87EE7AF79}" src="https://github.com/user-attachments/assets/40388e99-79e7-4209-b239-36d4abf83d07" />

<img width="960" height="540" alt="{10D44FE0-D9C5-4F1E-BE29-E9781483C2BF}" src="https://github.com/user-attachments/assets/813b0014-5340-4ed4-9dee-a1370cc6036d" />

3. Chạy Docker Compose

<img width="833" height="68" alt="{7CF10815-3958-463B-9BBD-D6BCC44D6932}" src="https://github.com/user-attachments/assets/9b54aabf-dc89-4545-a1e3-ca5e4d35852a" />

4. Cài đặt WordPress

<img width="960" height="540" alt="{9E194C65-AD03-4407-98E2-7C0AC3D6F160}" src="https://github.com/user-attachments/assets/a765eee8-7d4b-4de0-bbc5-82923e9e00ff" />
<img width="960" height="540" alt="{813BD11E-7199-4BA9-9329-2A0C65BD2F47}" src="https://github.com/user-attachments/assets/e5df41de-1c33-4241-a9fd-7201a19fd21b" />
<img width="960" height="540" alt="{0EA1F1A2-F586-4072-9C54-416A4B0C31D4}" src="https://github.com/user-attachments/assets/ac364696-7593-4701-9941-c2f2a75d0e39" />

5. Sử dụng cloudflare tunnel để public web này lên 1 sub-domain
   
<img width="960" height="540" alt="{F7C20238-7704-4AA2-8943-EDD5B033A6AB}" src="https://github.com/user-attachments/assets/dfa39f02-7361-4b02-a387-069f72520521" />

<img width="569" height="398" alt="{D7CFC0DD-DFEB-43E3-9612-3366B5BAA894}" src="https://github.com/user-attachments/assets/46eb1a09-91c9-46df-9f03-ccc65e21cdf3" />

6. Bây giờ làm nội dụng bài tập

 - Đăng nhập admin -> Mở https://localhost:8080/wn-admin

   - Tạo 1 bài viết trong wordpress giới thiệu về bản thân sinh viên: thông tin cá nhân, sở thích, ... bài viết có thể chứa hình ảnh, âm thanh, video, ...
     
<img width="960" height="540" alt="{4122A024-156F-428A-9BA4-EEE6789FAFE7}" src="https://github.com/user-attachments/assets/5a13f558-1e92-4401-a9f5-0f85d20f4512" />

   - Tạo 1 bài viết trong wordpress giới thiệu về ngành học mà em yêu thích trong trường TNUT. bài viết phải chứa hình ảnh, video, ..
     
<img width="960" height="540" alt="{21E708B2-7894-4E86-8A08-8A01E4C62898}" src="https://github.com/user-attachments/assets/b9f99a5a-7706-46ab-a506-b73eb13a8311" />

<img width="960" height="540" alt="{67E0430F-C308-4184-96BD-74AD26829DDA}" src="https://github.com/user-attachments/assets/fe8084e4-662a-447f-810c-667c51960360" />

7. Nhận xét việc sử dụng mã nguồn mở wordpress để tạo website (tốn công sức thế nào, dễ/khó dùng ra sao, tốn kém tài nguyên(ssh/ram) của máy chủ ra sao,....)
