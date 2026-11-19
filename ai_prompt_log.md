# AI Prompt Log – SkyWay Flight Booking System

### Prompt 01 – Tìm hiểu cách hiển thị logo

**Câu hỏi:**

> `<header><p>Đại lý vé máy bay SkyWay</p></header>` – chỗ này để logo thì dùng thẻ gì?

**Lý do sử dụng:**

Tìm hiểu cách chèn logo vào khu vực Header bằng HTML đúng ngữ nghĩa.

**Kiến thức tiếp thu:**

- Sử dụng `<img>` để hiển thị logo.
- Thuộc tính `src` xác định đường dẫn hình ảnh.
- Thuộc tính `alt` hỗ trợ khả năng truy cập (Accessibility).
- Có thể kết hợp `<a>` để tạo liên kết về trang chủ.

### Prompt 02 – Quy ước giá trị cho hạng ghế

**Câu hỏi:**

> `<option value="">Phổ thông</option>`  
> `<option value="">Hạng nhất</option>`  
> `<option value="">Thương gia</option>`  
>
> đưa cho mình các value cho đúng với hạng ghế

**Lý do sử dụng:**

Xác định giá trị `value` phù hợp cho các lựa chọn hạng ghế, giúp dữ liệu gửi đến Backend rõ ràng và nhất quán.

**Kiến thức tiếp thu:**

- `economy`: Phổ thông.
- `business`: Thương gia.
- `first_class`: Hạng nhất.
- Không nên sử dụng cùng một giá trị rỗng cho các lựa chọn hợp lệ.

### Prompt 03 – Thiết lập lựa chọn mặc định

**Câu hỏi:**

> option có defaut không

**Lý do sử dụng:**

Tìm hiểu cách đặt giá trị mặc định cho `<select>` và yêu cầu người dùng chủ động chọn hạng ghế.

**Kiến thức tiếp thu:**

- Thuộc tính `selected` dùng để chọn một `<option>` mặc định.
- Thuộc tính `disabled` vô hiệu hóa một lựa chọn.
- Có thể kết hợp `value=""`, `disabled`, `selected` và `required` để tạo lựa chọn hướng dẫn, yêu cầu người dùng chọn giá trị hợp lệ.

### Prompt 04 – Sinh dữ liệu chuyến bay giả định

**Câu hỏi:**

> tạo giúp 5 chuyến bay có hoãn/hủy và các chuyến bay cùng giờ

**Lý do sử dụng:**

Cần dữ liệu giả định để kiểm thử bảng lịch bay, đặc biệt là các trường hợp sử dụng `colspan` và `rowspan`.

**Dữ liệu AI cung cấp:**

| Mã chuyến | Hành trình | Giờ bay | Tình trạng |
|---|---|---|---|
| VN123 | Hà Nội → TP.HCM | 08:00 | Đúng giờ |
| VJ456 | Hà Nội → Đà Nẵng | 08:00 | Đúng giờ |
| QH789 | TP.HCM → Phú Quốc | 10:30 | Hoãn đến 12:00 |
| VN234 | Hà Nội → Nha Trang | 13:45 | Đã hủy |
| VJ567 | Đà Nẵng → Hà Nội | 16:20 | Đúng giờ |

**Kiến thức tiếp thu:**

- `rowspan="2"` dùng để gộp ô thời gian của hai chuyến bay cùng giờ.
- `colspan="4"` dùng để tạo hàng thông báo trải dài qua bốn cột.
- Khi gộp ô cần điều chỉnh số lượng `<td>` tương ứng để không làm lệch cấu trúc bảng.

