# Lab 2 — Thiết kế máy trạng thái hữu hạn (FSM)

*đang cập nhật...*

<!--

## Đề bài
<!-- phát hiện 3 bit liên tiếp 101 (cho phép overlap), dùng FF-D, làm cả Moore và Mealy; chuỗi X mẫu -> Y mẫu; ghi chú mô phỏng/DE2 nếu GV yêu cầu 

## Mục tiêu lab


## Mình đã làm gì?
### 0. Ý tưởng chung
<!-- mạch cần "nhớ" gì qua từng bit? Vì sao FF-D không cần bảng kích thích riêng? 

### 1. Máy trạng thái kiểu Moore
#### 1.1 Sơ đồ chuyển trạng thái

#### 1.2 Bảng chuyển trạng thái và mã hóa trạng thái

#### 1.3 Phương trình ngõ vào FF-D và ngõ ra Z

#### 1.4 Vẽ mạch trên Quartus


### 2. Máy trạng thái kiểu Mealy
#### 2.1 Sơ đồ chuyển trạng thái

#### 2.2 Bảng chuyển trạng thái và mã hóa trạng thái

#### 2.3 Phương trình ngõ vào FF-D và ngõ ra Z

#### 2.4 Vẽ mạch trên Quartus


## Kết quả mô phỏng
<!-- chu kỳ CLK, nhóm tín hiệu, các chuỗi X đã test, đối chiếu Y với chuỗi mẫu của đề 
### Moore

### Mealy


## So sánh Moore và Mealy
<!-- số trạng thái, số FF, độ phức tạp ngõ ra, thời điểm Z lên 1 


## Khó khăn và cách giải quyết
| Khó khăn | Cách giải quyết |
|:---|:---|
|  |  |

## Mình đã học được gì?


**GHI CHÚ THÔ KHI ĐANG LÀM (xóa khi viết xong)**
- Trong phần thiết kế FSM kiểu Mealy, ban đầu mình để grid size mặc định (nhớ không nhầm là bằng 1/4 chu kỳ clock), dạng sóng của output Z sai hoàn toàn. Sau đó mình mới chỉnh lại grid size bằng đúng chu kỳ clock, và chạy lại mô phỏng, thì dạng sóng của output Z mới đúng với những gì kì vọng. Sau đó mình có hỏi lại giảng viên và cũng đã được xác nhận là ở bài tập này thì ta sẽ giả sử mỗi bit interval sẽ nằm trọn trong một chu kỳ clock. Tức là phải đảm bảo cho X ổn định xung quanh cạnh lên của clock.
- Đang gặp vấn đề: Quartus chưa nhận diện được USB-Blaster của KIT Altera DE2 để nạp thiết kế.