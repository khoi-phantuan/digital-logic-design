# Lab 1 — Thiết kế mạch đếm đồng bộ có khả năng nạp giá trị ban đầu đồng bộ

Đây chỉ là bài tập thêm của Lab 1.

Ngược lại với bài tập chính yêu cầu việc nạp giá trị phải là bất đồng bộ thông qua chân PRE và CLR (tích cực mức thấp) của FF, bài tập này yêu cầu việc nạp giá trị phải là đồng bộ (thông qua đường input của T-FF).

Việc ta cần làm là xóa bỏ logic nạp bất đồng bộ của mạch cũ, và thêm logic mới: **Cho phép mạch lựa chọn có nạp giá trị input vào hay không tại từng thời điểm, thông qua tín hiệu điều khiển EN**.