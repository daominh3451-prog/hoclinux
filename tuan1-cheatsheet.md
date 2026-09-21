# Ubuntu Server CLI Cheat Sheet (Theo chuẩn Ubuntu Docs)

## 1. Điều hướng thư mục (Navigation)
- `pwd`: Hiển thị đường dẫn thư mục hiện tại bạn đang đứng.
- `ls`: Liệt kê các file và thư mục trong thư mục hiện tại.
- `ls -l`: Xem danh sách chi tiết (kèm quyền, chủ sở hữu, kích thước, ngày tháng).
- `ls -a`: Hiển thị tất cả, bao gồm cả các file ẩn (bắt đầu bằng dấu chấm `.`).
- `ls -la`: Xem chi tiết toàn bộ bao gồm cả file ẩn.
- `cd <thu_muc>`: Di chuyển đến thư mục chỉ định.
- `cd ..`: Lùi lại thư mục cấp trên (cha).
- `cd ~`: Quay trở về thư mục cá nhân (Home).
- `cd -`: Quay lại thư mục vừa đứng trước đó.
- `cd /`: Nhảy thẳng về thư mục gốc (Root) của hệ thống.

## 2. Quản lý hệ thống file (Working with the filesystem)
- `mkdir <ten>`: Tạo một thư mục mới.
- `rmdir <ten>`: Xóa một thư mục trống.
- `tree`: Hiển thị cây cấu trúc thư mục dạng phân cấp.
- `tree -L n`: Hiển thị cây thư mục giới hạn đến độ sâu cấp `n`.

## 3. Thao tác với File (Working with files)
- `touch <ten_file>`: Tạo file rỗng mới hoặc cập nhật thời gian của file.
- `cp <nguon> <dich>`: Sao chép file từ nguồn sang đích.
- `cp -a <nguon> <dich>`: Copy đệ quy toàn bộ thư mục, giữ nguyên quyền hạn và metadata.
- `mv <cu> <moi>`: Đổi tên hoặc di chuyển file/thư mục.
- `rm <ten_file>`: Xóa một file.
- `rm -r <thu_muc>`: Xóa đệ quy một thư mục không trống và toàn bộ nội dung bên trong.
- `cat <file>`: In toàn bộ nội dung file ra màn hình.
- `less <file>`: Xem nội dung file từng trang một (dùng phím q để thoát).
- `head -n 20 <file>`: Xem 20 dòng đầu tiên của file.
- `tail -n 20 <file>`: Xem 20 dòng cuối cùng của file.
- `wc -l <file>`: Đếm tổng số dòng của một file.

## 4. Người dùng, Nhóm và Phân quyền (Users, groups, and permissions)
- `chmod <quyen> <file>`: Thay đổi quyền hạn của file (ví dụ: `chmod 755`, `chmod +x`).
- `chown <user>:<group> <file>`: Thay đổi chủ sở hữu và nhóm sở hữu file.
- `umask`: Xem hoặc thiết lập mặt nạ quyền mặc định cho file mới.
- `sudo <lenh>`: Chạy một lệnh với quyền quản trị viên cao nhất.

## 5. Tìm kiếm (Searching)
- `grep "<tu_khoa>" <file>`: Tìm kiếm các dòng chứa từ khóa khớp trong file.
- `grep /etc/passwd`: Tra cứu thông tin tài khoản người dùng hệ thống.
- `find <thu_muc> -name "<ten>"`: Tìm kiếm file hoặc thư mục theo tên.
- `which <lenh>`: Hiển thị đường dẫn tuyệt đối của câu lệnh thực thi.

## 6. Chuyển hướng đầu vào/đầu ra (Redirecting input and output)
- `cmd > file`: Ghi đè kết quả của lệnh `cmd` vào file (tạo mới hoặc xóa nội dung cũ).
- `cmd >> file`: Ghi nối tiếp (append) kết quả vào cuối file.
- `cmd < file`: Lấy nội dung file làm đầu vào cho lệnh `cmd`.
- `cmd > /dev/null`: Ẩn toàn bộ kết quả trả về (vứt vào thùng rác hệ thống).
