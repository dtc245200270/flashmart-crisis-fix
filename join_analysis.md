Khi thực hiện LEFT JOIN, các bản ghi thuộc bảng bên trái không có giao dịch tương ứng ở bảng bên phải vẫn được giữ lại với các trường của bảng bên phải mang giá trị NULL. 

Hàm COUNT(*) tính toàn bộ số dòng được tạo ra mà không phân biệt giá trị của từng cột, khiến khách hàng chưa mua hàng (như Charlie) bị đếm nhầm thành 1 đơn. Trong khi đó, COUNT(o.order_id) chỉ đếm các giá trị khác NULL trên khóa chính của bảng Orders. Nhờ vậy, đối với khách hàng chưa từng phát sinh giao dịch, kết quả trả về chính xác là 0 đơn hàng.
