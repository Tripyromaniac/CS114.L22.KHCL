# Bài tập tuần 6: 
**Câu hỏi**: Tìm ví dụ về bài toán Linear regression ***trong thực tế***

## Vd1: Dự đoán lượt xem của 1 video trên nền tảng Youtube:
- **Input:** số lượng subcribers cũa kênh (kiểu int)
- **Output:** số lượng view có thể đạt được của video sau một khoảng thời gian (kiểu int) 
- **Nguồn dữ liệu:** 
  + Ghi nhận từ thực tế lượt view đạt được của từng video của kênh trong một khoảng thời gian sau khi post lên
- **Xử lý dữ liệu:**
  + Vì các dữ liệu liên quan đến thông số lượt tương tác người dùng nên miền giá trị các dữ liệu không có sự chênh lệch lớn không đòi hỏi các phương pháp xử lý dữ liệu đặc biệt

## Vd2: Dự đoán năng suất cây trồng:
- **Input:** các chỉ số về đất, nước, độ ẩm đất, các khoáng chất trong đất... kiểu float
- **Output:** khối lượng sản phẩm trên 1 ha (kiểu float)
- **Cách thu thập data:**
  + Dữ liệu được thu thập thông qua đo lường thực tế các yếu tố đất, nước... (kiểu float)
  + Dữ liệu về ảnh hưởng của phân bón lên cây được thu thập thông qua các báo cáo của bộ nông nghiệp và phát triển nông thôn (kiểu float)
- **Xử lý data:**
  + Những dữ liệu có miền giá trị chênh lệch nhau qua lớn trước khi đưa vào model sẽ được chuyển đổi để chênh lệch không còn đáng kể 
  + Loại bỏ giá trị null ở những bộ dữ liệu đo lường năng suất chỉ dựa vào 
  + chuyển dữ liệu dạng bảng về dạng file .csv

## Vd3: Dự đoán tỷ lệ trẻ sinh ra bị khuyết tật bẩm sinh:
- **Input:** 
  + Chỉ số cơ thể của thai phụ (kiểu float)
  + Khả năng mắc các bệnh ảnh hưởng đến thai nhi (kiểu bool) 
  + Thói quen sinh hoạt hằng ngày (kiểu bool) (vd: có hút thuốc ko, có nghiện rượu không,...) 
- **Output:** Phần trăm khả năng thai nhi dị tật (kiểu float)
- **Cách thu thập data:**
  + Thông qua hồ sơ bệnh án của những thai phụ đã sinh nở thành công
  + Dữ liệu của người được dự đoán được đo lường thông qua những lần khám thai định kì
- **Xử lý data:**
  + Dữ liệu kiểu float có thể xảy ra chênh lệch miền giá trị đòi hỏi phải chuyển đổi để các thông số có miền giá trị 
  + Dự liệu kiểu bool sẽ được chuyển về dạng int là 0/1 biểu thị cho có/không
  + Bộ data sẽ được chuyển sang file .csv trước khi đưa vào train model

## Vd4: Dự đoán doanh thu năm của doanh nghiệp
- **Input:** 
  + Doanh thu hằng hàng tháng của doanh nghiệp trong năm (kiểu float) 
  + Tác động của các sự kiện đặc biệt tương ứng mốc thời gian của năm (kiểu int)
  + Các khoảng chi tiêu hàng tháng của doanh nghiệp (kiểu float)
- **Output:** doanh thu năm tiếp theo của doanh nghiệp
- **Cách thu thập data:**
  + Ghi nhận báo cáo doanh thu hằng năm của doanh nghiệp
  + Hóa đơn chi phí thanh toán các khoản duy trì hoạt động doanh nghiệp 
  + Báo cáo kế hoạch của doanh nghiệp về tác động của các sự kiện
- **Xử lý data:**:
  + Xóa các giá trị null ở cột tác động của các sự kiện đối với những tháng không có biến động gì đặc biệt
  + Chuyển kiểu bool ở dữ liệu về tác động của các sự kiến sang kiểu int với 1/0 biểu thị cho tích cực/tiêu cực 
