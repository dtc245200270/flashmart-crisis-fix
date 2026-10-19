## Câu hỏi 1:
- **Prompt:** Sự khác biệt giữa INNER JOIN và LEFT JOIN trong bài toán thống kê số lượng đơn hàng của khách hàng là gì?
- **Tóm tắt phản hồi:** INNER JOIN chỉ giữ lại tập giao (giao dịch đã diễn ra), làm mất các khách hàng chưa mua hàng. LEFT JOIN bảo toàn toàn bộ bảng khách hàng (Driving table), cho phép nhận diện nhóm chưa phát sinh đơn.

## Câu hỏi 2:
- **Prompt:** Tại sao dùng COUNT(*) trong LEFT JOIN lại cho kết quả sai lệch so với COUNT(column_name)?
- **Tóm tắt phản hồi:** COUNT(*) đếm số hàng trả về của kết quả truy vấn kể cả khi dòng đó chứa giá trị NULL, còn COUNT(column_name) bỏ qua các ô có giá trị NULL.

## Câu hỏi 3:
- **Prompt:** Nguyên lý của kỹ thuật Anti-Join với cú pháp LEFT JOIN ... WHERE column IS NULL là gì?
- **Tóm tắt phản hồi:** LEFT JOIN sinh ra giá trị NULL cho bảng phụ nếu không tìm thấy liên kết phù hợp. Mệnh đề WHERE ... IS NULL lọc chính xác những bản ghi không có liên kết đó.
