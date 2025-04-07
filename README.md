# Customer_Segmentation
Đây là bài toán Phân khúc khách hàng bằng cách sử dụng RFM và KMeans,  các bước cụ thể:
- Thực hiện biến đổi dữ liệu để tạo ra dataframe với cột customer_id và 3 cột feature theo mô hình RFM
  - Recency: Ngày mua hàng gần nhất
  - Frequency: Tần suất mua hàng
  - MontaryValue: Giá trị mà khách hàng đã bỏ ra
- Chuẩn hóa dữ liệu để gần nhất với normal distribution bằng cách tối ưu điểm skewness về ~ 0 bằng 1 trong 4 phương pháp:
  - Log Transformation
  - Square Root Transformation
  - Box-Cox Transformation
  - Yeo-Johnson Transformation
- Scale dữ liệu bằng phương pháp Standard Scaling (phương pháp này tốt với dữ liệu được chuẩn hoá)
- Đưa dữ liệu vào mô hình KMeans:
  - Chọn số cụm bằng Elbow
- Áp dụng mô hình để phân cụm, đánh giá từng cụm được phân
