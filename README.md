# **Dự án Phân nhóm Khách hàng**

## **Tổng quan**
Dự án này tập trung vào việc phân nhóm khách hàng cho một công ty nhằm thúc đẩy hoạt động kinh doanh bằng cách triển khai các chiến lược phù hợp cho từng nhóm khách hàng. Bằng cách xác định các yếu tố quan trọng và áp dụng các kỹ thuật phân cụm, chúng ta có thể phân khách hàng dựa trên hành vi mua sắm và các chỉ số khác, từ đó giúp tạo ra các chiến lược tiếp thị cá nhân hóa.

## **Thông tin dự án**

### **Tên dự án**: Phân nhóm Khách hàng  

### **Mục tiêu của dự án**
Mục tiêu của dự án là phân nhóm khách hàng thành các nhóm khác nhau dựa trên các yếu tố như tần suất mua hàng, số tiền chi tiêu và thời gian từ lần mua gần nhất. Việc phân nhóm này sẽ giúp công ty xây dựng các chiến lược tiếp thị cụ thể cho từng nhóm khách hàng.

## **Quy trình thực hiện**

### 1. **Nhập thư viện và tải dữ liệu**
   - Nhập các thư viện Python cần thiết (ví dụ: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`).
   - Tải dữ liệu giao dịch của khách hàng để phân tích.

### 2. **Hiểu dữ liệu**
   - Hiển thị các thông tin mô tả về dữ liệu để hiểu rõ hơn về sự phân bố của các biến chính (min, max, mean, std).
   - Trả lời các câu hỏi liên quan về bộ dữ liệu.

### 3. **Chuẩn bị dữ liệu**
   - Làm sạch dữ liệu và xử lý các giá trị thiếu nếu có.
   - Tạo các biến:
     - **Recency**: Số ngày kể từ lần mua hàng gần nhất.
     - **Frequency**: Số lần giao dịch của mỗi khách hàng.
     - **Monetary Value (Amount)**: Tổng số tiền chi tiêu của khách hàng.
   - Trực quan hoá các biến này bằng cách sử dụng biểu đồ QQ-plot.

### 4. **Mô hình hóa – k-Means Clustering**
   - Áp dụng thuật toán **k-means clustering** lên dữ liệu đã được chuẩn hoá (`Recency`, `Frequency`, `Amount`) sau khi thực hiện log transformation và standardization.
   - Trực quan hoá các cụm và đưa ra nhận xét.

### 5. **Tìm Insight từ các cụm**
   - Phân tích các nhóm khách hàng với từng giá trị **K** khác nhau.
   - Trực quan hóa phân bố của khách hàng và tổng số tiền chi tiêu cho từng cụm tương ứng với mỗi giá trị K.

### 6. **Phân tích sâu hơn từng cụm**
   - Thực hiện phân tích sâu hơn để hiểu rõ hơn hành vi của các nhóm khách hàng trong từng cụm.

## **Yêu cầu**

### **Thư viện/Các gói cần cài đặt**
Để chạy dự án này, bạn cần các thư viện sau:
```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
pip install -r requirements.txt

