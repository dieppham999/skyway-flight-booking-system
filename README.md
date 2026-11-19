# SkyWay Flight Booking System

## 1. Giới thiệu

Dự án thực hành xây dựng giao diện đặt vé máy bay và bảng lịch trình chuyến bay cho đại lý SkyWay.

Mục tiêu là cải thiện cấu trúc HTML cũ, áp dụng Semantic HTML5, xây dựng biểu mẫu nhập liệu có kiểm tra dữ liệu và trình bày bảng lịch bay khoa học.

**Vai trò:** Frontend Developer  
**Công nghệ:** HTML5 thuần  
**Bài thực hành:** Số hóa quy trình đặt vé tại Đại lý SkyWay

## 2. Mục tiêu

- Hiểu và sử dụng các thẻ HTML5 Form.
- Áp dụng HTML5 Validation để kiểm tra dữ liệu.
- Sử dụng các thẻ Semantic Table.
- Thực hành gộp ô bằng `colspan` và `rowspan`.
- Cải thiện trải nghiệm nhập liệu và khả năng truy cập.
- Hiểu nguyên lý gửi dữ liệu bằng GET và POST.

## 3. Chức năng

### 3.1. Biểu mẫu đặt vé

Cho phép người dùng nhập:

- Họ và tên.
- Số điện thoại.
- Email.
- Giới tính.
- Ngày bay.
- Chuyến bay.
- Hạng ghế: Phổ thông, Thương gia, Hạng nhất.

Áp dụng các thuộc tính `required`, `placeholder` và kiểu dữ liệu HTML5 phù hợp để hỗ trợ kiểm tra thông tin trước khi gửi.

### 3.2. Bảng lịch trình chuyến bay

Hiển thị tối thiểu 5 chuyến bay với các thông tin:

- Mã chuyến bay.
- Điểm khởi hành và điểm đến.
- Thời gian bay.
- Tình trạng chuyến bay.

Sử dụng `thead`, `tbody`, `tfoot`, `th`, `td` để tổ chức dữ liệu.

Áp dụng `colspan` để hiển thị thông báo hoãn/hủy và `rowspan` để nhóm các chuyến bay cùng giờ.

## 4. Công nghệ sử dụng

- HTML5
- HTML5 Form Validation
- Semantic HTML

Không sử dụng CSS hoặc JavaScript.

## 5. Cấu trúc thư mục

```text
skyway-flight-booking-system/
├── booking_system.html
├── ai_prompt_log.md
└── README.md
```

**Giải thích:**

- `booking_system.html`: Giao diện Form và Table.
- `ai_prompt_log.md`: Nhật ký câu hỏi và quá trình sử dụng AI.
- `README.md`: Tài liệu giới thiệu và hướng dẫn dự án.

## 6. Hướng dẫn chạy

1. Clone repository về máy.
2. Mở thư mục dự án bằng VS Code.
3. Mở file `booking_system.html` bằng Chrome hoặc Edge.
4. Kiểm tra Form đặt vé và bảng lịch bay.

Không cần cài đặt thư viện hay máy chủ để xem giao diện HTML tĩnh.

## 7. Kiểm thử

Checklist nghiệm thu:

- [ ] Không thể gửi Form khi thiếu trường bắt buộc.
- [ ] Email sai định dạng bị trình duyệt cảnh báo.
- [ ] Các Label liên kết đúng với trường nhập liệu.
- [ ] Chọn được giới tính, ngày bay, chuyến bay và hạng ghế.
- [ ] Bảng hiển thị tối thiểu 5 chuyến bay.
- [ ] `colspan` không làm sai số lượng cột.
- [ ] `rowspan` không làm lệch các hàng.
- [ ] Không sử dụng JavaScript.

## 8. Kiến thức trọng tâm

### GET và POST

- `GET`: Dữ liệu biểu mẫu được mã hóa vào URL dưới dạng query string.
- `POST`: Dữ liệu được gửi trong phần thân HTTP request, không hiển thị trực tiếp trên thanh địa chỉ như GET.

POST phù hợp hơn với việc gửi thông tin đặt vé. Tuy nhiên, POST không tự mã hóa dữ liệu; cần sử dụng HTTPS để bảo vệ thông tin khi truyền.

### Phân biệt th và td

- `<th>`: Ô tiêu đề, mang ý nghĩa ngữ nghĩa cho hàng hoặc cột.
- `<td>`: Ô chứa dữ liệu thông thường.

### Phân biệt colspan và rowspan

- `colspan`: Gộp nhiều cột thành một ô.
- `rowspan`: Gộp nhiều hàng thành một ô.

### HTML5 Validation

Sử dụng các thuộc tính như `required`, `type="email"` và các ràng buộc phù hợp nhằm kiểm tra dữ liệu ở phía trình duyệt.

Validation phía trình duyệt không thay thế việc kiểm tra dữ liệu trên Backend.

## 9. Quy tắc sử dụng AI

AI chỉ được sử dụng để:

- Giải thích kiến thức HTML.
- Gợi ý phương án thiết kế.
- Sinh dữ liệu chuyến bay giả định.
- Phân tích lỗi và đề xuất trường hợp kiểm thử.

Học viên tự triển khai mã nguồn và ghi lại các câu hỏi đã sử dụng trong `ai_prompt_log.md`.

## 10. Kết quả cần đạt

- Giao diện HTML có cấu trúc ngữ nghĩa rõ ràng.
- Form hỗ trợ kiểm tra dữ liệu HTML5.
- Bảng lịch bay hiển thị đúng khi gộp hàng và cột.
- Hiểu và giải thích được các thẻ, thuộc tính đã sử dụng.

**Lưu ý:** Đây là bài thực hành Frontend HTML tĩnh. Chức năng lưu trữ hoặc xử lý đặt vé thực tế phụ thuộc vào Backend và không thuộc phạm vi triển khai của bài tập.