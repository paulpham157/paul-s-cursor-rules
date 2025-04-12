# Paul's Cursor Rules

## Giới thiệu

- Repo này tổng hợp settings, các kinh nghiệm cá nhân của tôi trong quá trình sử dụng Cursor IDE trong việc coding.
- Repo này public hoàn toàn dưới dạng giấy phép nguồn mở MIT.
- Bạn không cần phải xin phép ai khi sử dụng/sửa đổi nó với mục đích cá nhân.
- Trong trường hợp sử dụng thương mại, bạn cần dẫn nguồn rõ ràng, không sửa đổi đến đường dẫn <a href="https://github.com/paulpham157/paul-s-cursor-rules/blob/main/LICENSE">LICENSE nguồn mở từ repo này</a> và toàn bộ các giấy phép từ các nguồn khác mà repo này sử dụng.


## Chỉ dùng 1 trong 2 cách sau:

### ⭐ Hướng dẫn sử dụng Cách 2: MỚI ⭐
Sử dụng các file trong thư mục `2`

- KHÔNG cần phải set global_rule gì đặc biệt trong Cursor settings => Rules => User Rules. Nếu có thì chỉ cần đơn giản như "Always respond in Vietnamese." cũng được
- (Nếu bạn đã từng dùng cách 1) với cách 2 này, không cần phải tạo file `scratchpad.md`, Cursor sẽ tự tạo
- Copy file `.cursorrules` vào workspace của bạn
- Trong Cursor mở cửa sổ chat mới, chọn agent, add context file `.cursorrules` (hoặc @ nó vào, nếu tab đang mở là file `.cursorrules` luôn thì nó sẽ tự add, không cần làm gì nữa cả)
- Bắt đầu làm việc. Để cho chắc, câu đầu tiên bạn có thể hỏi nó "đã rõ công việc của mình chưa?" để xác nhận lại
- Rule này hoạt động tốt nhất ở chế độ agent, với các model thinking claude-3.7-sonnet (không cần MAX), gemini-2.5-pro (không cần MAX)
- Sau khoảng chục lần đò đưa thì bạn nên bảo cursor là "ok, bây giờ bạn làm rất tốt, bây giờ bạn tổng hợp bài học đi và làm sạch những task đã done trong scratchpad để còn làm task mới nữa". Xong rồi nó summary lại file `scratchpad.md`, bạn mở 1 đoạn chat mới và bảo "chào nhân viên mới, hãy làm tiếp công việc còn lại". Việc này để tránh memory leaking khi mà file `scratchpad.md` càng to thì lượng context đưa vào càng nhiều, mà mỗi model lại chỉ có limit context length nhất địng thôi. Mặc dù chat tiếp thì vẫn được thôi nhưng tốt nhất là sang 1 đoạn chat mới.

### Hướng dẫn sử dụng Cách 1: CŨ
Sử dụng các file trong thư mục `1`

#### Setup rules

- Copy nội dung global_rule vào Cursor settings => Rules => User Rules
- Mỗi dự án, tạo một file `.cursorrules` và dán nội dung file devin_rule-v1 vào
- Với mỗi dự án chuyên biệt, nếu cần set những rule cụ thể hơn, ví dụ typescript thì cần phải viết như này như này; hãy tham khảo folder framework_rules. Tạo folder .cursor/rules trong dự án của bạn và thêm copy những file rule bạn cần vào trong đó.

#### Tricks

- Sử dụng tốt nhất với Agent mode, claude-3.7-sonnet thinking
- Thay vì prompt "tôi muốn bạn làm việc ABC" thì hãy prompt "hãy lên lịch/kế hoạch từng bước để làm việc ABC"
- notepads... là gì? dùng như nào? (trong phiên bản gần đây, Cursor đã bỏ)
- MCP... là gì? dùng như nào? (có quá nhiều bác đã lên bài rồi ^^ e k nói lại nữa)
- Các settings khác... (đang cập nhật)

## Nguồn

- Hiểu biết không tự nhiên sinh ra, nó là kết quả sau một quá trình học tập. Và trong quá trình đó, tôi đã sử dụng các nguồn tài liệu sau:
- File devin_rule-v1: https://github.com/grapeot/devin.cursorrules giấy phép <a href="https://github.com/grapeot/devin.cursorrules/blob/master/LICENSE">MIT LICENSE</a>. Họ đang chuẩn bị cho 1 bản cập nhật mới, tốt hơn.
- Folder framework_rules: https://github.com/PatrickJS/awesome-cursorrules giấy phép <a href="https://github.com/PatrickJS/awesome-cursorrules/blob/main/LICENSE">CC0 1.0 Universal</a> đây cũng là một loại giấy phép nguồn mở. <a href="https://creativecommons.org/publicdomain/zero/1.0/">Tìm hiểu thêm</a>.
- Nguyên bản tất cả các giấy phép nằm trong thư mục licenses.

## Đóng góp

- Vì đây là một sản phẩm cộng đồng, nên không có điều kiện nào đặc biệt nào khi tham gia đóng góp mã nguồn.
- Hãy fork repo này về và chỉnh sửa, thêm mới các rule mà bạn cảm thấy ok hơn. Sau đó tạo pull request. Tôi sẽ merge khi nào tôi rảnh.
- Một khi được merge, tên bạn sẽ xuất hiện trong danh sách những người đóng góp. Cảm ơn bạn <3

## Những người đóng góp

<!-- readme: contributors -start -->
<table>
	<tbody>
		<tr>
            <td align="center">
                <a href="https://github.com/paulpham157">
                    <img src="https://avatars.githubusercontent.com/u/68021190?v=4" width="100;" alt="paulpham157"/>
                    <br />
                    <sub><b>Paul Pham 157</b></sub>
                </a>
            </td>
		</tr>
	<tbody>
</table>
<!-- readme: contributors -end -->

## License

This project is open source and available under the <a href="https://github.com/paulpham157/paul-s-cursor-rules/blob/main/LICENSE">MIT License</a>.
