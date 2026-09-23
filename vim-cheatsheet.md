# Cheat-sheet Trình soạn thảo Vim

## 1. Hai chế độ cơ bản trong Vim
- **Chế độ lệnh (Command Mode):** Chế độ mặc định khi vừa mở file, dùng để điều khiển, di chuyển và thực hiện lệnh.
- **Chế độ soạn thảo (Insert Mode):** Dùng để gõ chữ và chỉnh sửa văn bản.

## 2. Phím chuyển đổi qua lại chế độ
- Bấm **`i`**: Chuyển sang chế độ gõ chữ (hiện chữ `-- INSERT --` ở góc dưới màn hình).
- Bấm **`Esc`**: Thoát chế độ gõ chữ, quay về chế độ lệnh.

## 3. Bộ lệnh cứu mạng (Thoát và Lưu) - *Luôn bấm Esc trước khi gõ*
- `:wq` + `Enter`: Lưu lại nội dung file và thoát khỏi Vim[cite: 1].
- `:q!` + `Enter`: Thoát ngay lập tức mà **không lưu** bất kỳ thay đổi nào (dùng khi lỡ sửa hỏng)[cite: 1].
- `:w` + `Enter`: Chỉ lưu file mà không thoát.

## 4. Các phím thao tác nhanh (ở Chế độ lệnh)
- **`dd`**: Xóa hẳn dòng hiện tại[cite: 1].
- **`yy`**: Sao chép (copy) dòng hiện tại[cite: 1].
- **`p`**: Dán nội dung vừa copy xuống dòng phía dưới[cite: 1].
- **`u`**: Hoàn tác (Undo) lại thao tác vừa làm trước đó[cite: 1].
- **`/tu_khoa`**: Tìm kiếm từ khóa trong văn bản (nhấn Enter để tìm).

## 5. Ký hiệu giao diện
- Dấu **`~`** ở cột bên trái màn hình: Thể hiện đây là các dòng trống chưa có nội dung văn bản.
