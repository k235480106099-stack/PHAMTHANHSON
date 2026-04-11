Bài tập môn Hệ quản trị cơ sở dữ liệu-TEE560, Lớp: 59KMT

Họ tên: Phạm Thanh Sơn

Lớp:K59KMT.K01

MSSV: K235480106099

BÀI TẬP

1.Download và cài đặt SQL Server 2025, phiên bản Developer

Link tải: https://www.microsoft.com/vi-vn/sql-server/sql-server-downloads

Chọn phiên bản SQL Server 2025 Developer

Không chọn Azure (nặng, ko dùng đến), các tính năng mở rộng khác (feature) chọn tất cả

Cài đặt với 2 kiểu login (Mixed Mode): Windows Authentication (nhớ Add Current User) và SQL Server Authentication (username mặc định là sa, chỉ cần nhập mật khẩu 123 , nhớ nhập 2 chỗ: Enter password và Confirm password)
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/9d2b0ab4-e788-4408-acca-50d5cef5aa98" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0d83051c-2f29-489e-8c87-e11d99d12f78" />
2.Cấu hình cho SQL Server làm việc ở cổng động (Dynamic Port), TCP
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b9c3ecec-7c60-49f6-a510-4dbcd5c37957" />
3.Kiểm tra xem service SQL Server có đang running và mở đúng cổng đã chọn hay không?
<img width="1910" height="1076" alt="ảnh 3" src="https://github.com/user-attachments/assets/50ddaa5d-7542-4a29-a135-e66a02fc7f15" />
4.Cài đặt SQL Server Management Studio
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/322f02ee-98ac-4f51-bae2-2ef091860929" />
5.Chạy phần mềm ssms để Đăng nhập vào SQL Server bằng 2 cách
<img width="1918" height="1078" alt="ảnh 4" src="https://github.com/user-attachments/assets/9e8d129b-79d8-4fcb-b72a-3526c4c1f701" />
<img width="1918" height="1078" alt="ảnh 5 1" src="https://github.com/user-attachments/assets/527cfe68-a30b-4e60-88d3-bff6daef646e" />
<img width="1918" height="1078" alt="ảnh 5 2" src="https://github.com/user-attachments/assets/2f3426c8-ec33-49f0-b596-d6cb73914f94" />
6.Sử dụng giao diện đồ hoạ của ssms: Tạo cơ sở dữ liệu mới (create database) với tên tuỳ ý, chọn Path (nơi lưu trữ db) cho file lưu dữ liệu và file lưu log ở ổ đĩa khác với ổ C. mở path đã chọn xem 2 file đã tạo ra.
<img width="1918" height="1078" alt="ảnh 6 1" src="https://github.com/user-attachments/assets/3989869e-4795-4e33-a515-e185fb3eacfd" />
<img width="1918" height="1078" alt="ảnh 6 2" src="https://github.com/user-attachments/assets/6d797e89-7a23-413b-b189-a0f8d748364f" />
7.Sử dụng giao diện đồ hoạ của ssms: Tạo bảng dữ liệu (create and design table) với tên bảng tuỳ ý, có các trường dữ liệu phù hợp với dữ liệu của file data mẫu (CSV), với Khoá chính (Primary Key) là trường masv
<img width="1918" height="1078" alt="ảnh 7" src="https://github.com/user-attachments/assets/bbbe91ed-b101-4202-be64-00161463f3db" />
8.Sử dụng giao diện đồ hoạ của ssms: Tìm cách import dữ liệu từ file mẫu vào trong bảng vừa tạo.
<img width="1918" height="1078" alt="ảnh 8" src="https://github.com/user-attachments/assets/adb3a280-c682-4eb6-b287-06323f0d13c1" />
9.Mở cửa sổ mới để gõ lệnh trong ssms: GÕ lệnh để kiểm tra xem số dòng của bảng dữ liệu sau khi import.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e9720beb-113f-4463-8a68-fa68bf11715a" />
10.Trong cửa sổ mới để gõ lệnh: Gõ lệnh để thêm (insert) 1 row vào bảng, với dữ liệu là thông tin cá nhân của sv đang làm bài 
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e3fc51e7-7360-4ced-9eae-bbf2213c4853" />
11.Trong cửa sổ mới để gõ lệnh: Gõ lệnh để cập nhật(update) trường noisinh thành 'Sao Hoả' cho những dòng có noisinh và diachi đều là NULL.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/24ed7b01-f29c-4e2d-9afb-f017edd458ca" />
12.Sử dụng giao diện đồ hoạ của ssms: Tạo bảng SaoHoa gồm những sinh viên có nơi sinh ở 'Sao Hoả', keyword gợi ý: sử dụng 1 câu lệnh: SELECT + INTO
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f76de29f-3c1e-49b6-a37e-8067450a1f17" />
13.Gõ lệnh xoá (delete) trong bảng SaoHoa những sinh viên cùng họ với em
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/898db82b-aea5-400e-a881-478076f3d6db" />
14.Sử dụng giao diện đồ hoạ của ssms: Xuất toàn bộ kết quả của các bước 6,7,8,9,10,11,12,13 ra file dulieu.sql , keyword gợi ý: sử dụng tính năng GEN SCRIPT struct+data cho database
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/59ed8390-3141-4790-89d6-ec7fe5cb3753" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/40ef655e-8bdc-4780-ad17-2f57bc837e5e" />
15.Sử dụng giao diện đồ hoạ của ssms: Xoá csdl đã tạo, sau khi xoá thành công, kiểm tra tại path (path chọn ở bước 6) xem còn tồn tại 2 file của bước 6 không?
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/49374ccb-c13d-4dc1-a3ef-c88af46879b0" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/495015aa-6c21-4d3c-8165-4c09a7934af3" />
16.Tạo cửa sổ mới để gõ lệnh: mở file  của bước 14, chạy toàn bộ các lệnh này. REFRESH lại cây liệt kê các database => kiểm chứng kết quả được tạo ra tương đương với các bước 6,7,8,9,10,11,12,13.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/84505834-a44e-451f-b2bf-dafbac95c742" />
17.upload file
