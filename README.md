# PHÂN TÍCH VÀ KHẮC PHỤC LỖI CSS BOX MODEL

## Phần 1: Báo cáo phân tích (I/O)

**1. Kiểm tra bằng Inspect Element**

Nhấn F12, chọn lần lượt hai khung "Nội dung bài học" và "Danh sách video", sau đó vào tab Computed để kiểm tra 4 thành phần:

- Content: Khu vực hiển thị nội dung.
- Padding: Khoảng cách bên trong.
- Border: Đường viền của khung.
- Margin: Khoảng cách bên ngoài khung.

**2. Phân tích nguyên nhân**

Hai khung bị chồng lên nhau có thể do kích thước, Padding hoặc Margin chưa hợp lý.

Nếu chỉ tăng Margin mà không kiểm tra Padding thì khoảng cách có thể bị sai lệch, khiến giao diện bị giãn rộng hoặc mất cân đối.

## Phần 2: Thiết kế giải pháp

**1. Đề xuất chỉnh sửa trong bảng Styles**

Đối với khung Nội dung bài học:
- Padding: 15px.
- Margin-bottom: 20px.
- Width: 100%.

Đối với khung Danh sách video:
- Padding: 15px.
- Margin-top: 0px.
- Width: 100%.

**2. Cách khắc phục**

- Điều chỉnh Padding để nội dung không bị sát viền.
- Điều chỉnh Margin để tạo khoảng cách giữa hai khung.
- Kiểm tra lại chiều rộng và chiều cao của hai phần tử.
- Nếu vẫn bị chồng lấn, kiểm tra thêm thuộc tính Position.

**3. Kết quả mong đợi**

Hai khung Nội dung bài học và Danh sách video được tách biệt, không còn chồng lấn và vẫn giữ được bố cục ban đầu của trang PTIT-LMS.

