# Paul's Cursor Rules

### ⭐ Hướng dẫn sử dụng Cách 2: MỚI ⭐
Sử dụng các file trong thư mục `2`

- KHÔNG cần phải set global_rule gì đặc biệt trong Cursor settings => Rules => User Rules. Nếu có thì chỉ cần đơn giản như "Always respond in Vietnamese." cũng được
- (Nếu bạn đã từng dùng cách 1) với cách 2 này, không cần phải tạo file `scratchpad.md`, Cursor sẽ tự tạo
- Copy file `.cursorrules` vào workspace của bạn
- Trong Cursor mở cửa sổ chat mới, chọn agent, add context file `.cursorrules` (hoặc @ nó vào, nếu tab đang mở là file `.cursorrules` luôn thì nó sẽ tự add, không cần làm gì nữa cả)
- Bắt đầu làm việc. Để cho chắc, câu đầu tiên bạn có thể hỏi nó "đã rõ công việc của mình chưa?" để xác nhận lại
- Rule này hoạt động tốt nhất ở chế độ agent, với các model thinking claude-3.7-sonnet (không cần MAX), gemini-2.5-pro (không cần MAX)
- Sau khoảng chục lần đò đưa thì bạn nên bảo cursor là "ok, bây giờ bạn làm rất tốt, bây giờ bạn tổng hợp bài học đi và làm sạch những task đã done trong scratchpad để còn làm task mới nữa". Xong rồi nó summary lại file `scratchpad.md`, bạn mở 1 đoạn chat mới và bảo "chào nhân viên mới, hãy làm tiếp công việc còn lại". Việc này để tránh memory leaking khi mà file `scratchpad.md` càng to thì lượng context đưa vào càng nhiều, mà mỗi model lại chỉ có limit context length nhất địng thôi. Mặc dù chat tiếp thì vẫn được thôi nhưng tốt nhất là sang 1 đoạn chat mới.
