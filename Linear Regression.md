# Bài tập tuần 6: 
**Câu hỏi**: Tìm ví dụ về bài toán Linear regression ***trong thực tế***

## Vd 1: Dự đoán lượt xem của 1 video trên nền tảng Youtube:
Input: số lượng subcribers cũa kênh (kiểu int)
Output: số lượng view có thể đạt được của video sau một khoảng thời gian (kiểu int) 
Nguồn dữ liệu: Ghi nhận từ thực tế lượt view đạt được của từng video của kênh trong một khoảng thời gian sau khi post lên
Xử lý dữ liệu: Vì các dữ liệu liên quan đến thông số lượt tương tác người dùng nên miền giá trị các dữ liệu không có sự chênh lệch lớn không đòi hỏi các phương pháp xử lý dữ liệu đặc biệt

Dự đoán năng suất cây trồng:
Input: các chỉ số về đất, nước, độ ẩm đất, các khoáng chất trong đất... kiểu float
Output: khối lượng sản phẩm trên 1 ha (kiểu float)
Cách thu thập data:
- Dữ liệu được thu thập thông qua đo lường thực tế các yếu tố đất, nước... (kiểu float)
- Dữ liệu về ảnh hưởng của phân bón lên cây được thu thập thông qua các báo cáo của bộ nông nghiệp và phát triển nông thôn (kiểu float)
Xử lý data:
- Các giá trị về độ ẩm và nhiệt độ có miền giá trị chênh lệch so với chỉ số ác khoáng chất trong đất nên khi sử dụng để train sẽ xảy ra những trường hợp overfitting vậy nên trước khi vào model các số liệu sẽ được chuyển đổi để miền giá trị ko chênh lệch quá lớn 

Dự đoán khoảng thời gian sẽ xảy ra kẹt xe ở 1 tuyến đường trong ngày:
Input: dữ liệu về lưu lượng xe trung bình, chiều rộng tuyến đường, 
Output: thời gian sẽ diễn ra kẹt xe và thời gian kết thúc (

Dự đoán doanh thu năm của doanh nghiệp
Input: doanh thu hằng hàng tháng của doanh nghiệp trong năm (kiểu float), hệ số nhân của các sự kiện đặc biệt tương ứng mốc thời gian của năm, các khoảng chi tiêu hàng tháng của doanh nghiệp
Output: doanh thu năm tiếp theo của doanh nghiệp
Cách thu thập data: 
- Dựa vào báo cáo doanh thu hằng năm của doanh nghiệp 
