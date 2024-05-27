<span id="readme-top"></span>
<div style="text-align: center;">
   <h1 style="text-align: center;">Phân cụm thị trường cầu thủ bóng đá</h1>
   <p style="text-align: center;">Chương trình phân cụm thị trường cầu thủ bóng đá dựa vào các tiêu chí đánh giá</p>
</div>

## Mục lục

1. [Giới thiệu ứng dụng]
2. [Bắt đầu]
    * [Đầu tiên]
    * [Cài đặt]
        * [Cấu hình]
        * [Khởi chạy chương trình]

## Giới thiệu ứng dụng

Đây là một chương trình để thu thập, làm sạch và trực quan hóa dữ liệu cầu thủ bóng đá

## Bắt đầu

### Đầu tiên

* Đảm bảo đã cài đặt các thư viện cần thiết vị trí đầu của các file `.ipynb`

### Cài đặt

#### Cấu hình
Cài đặt các thư viện, plugin cần thiết cho mô tả và trực quan dữ liệu, khởi chạy file `.ipynb`

#### Khởi chạy chương trình

1. Clone the repo
   ```sh
   git clone https://github.com/tiennhat306/Clustering-Player-Market.git
    ```
2. Chạy các file `crawl_data.ipynb` sau đó `craw_detail.ipynb` trong thư mục `raw_data_train` và `raw_data_test` để thu thập dữ liệu huấn luyện và kiểm thử.
3. Chạy file `clean_data_train.ipynb` trong thư mục `clean_data_train`, `clean_data_test.ipynb` trong thư mục `clean_data_test` để tiến hành làm sạch dữ liệu huẩn luyện và kiểm thử: sửa lỗi định dạng, xóa dữ liệu bị thiếu, loại bỏ ngoại lệ cho tập huấn luyện. Xem cách xử lý và trực quan hoá sự thay đổi của phân bố dữ liệu trước và sau xử lý.
4. Tại thư mục `visualize_data`:
    -  Chọn file `univariate_data_visualization.ipynb`, chạy tất cả chương trình để xem các thống kê mô tả trực quan về dữ liệu đơn biến đối với một vài biến quan trọng.
    - Chọn file `variate_data_visualization.ipynb`, chạy tất cả chương trình để xem các mối quan hệ tiềm ẩn giữa các biến trong tập dữ liệu. Hay xem biểu đồ trực quan hoá không gian dữ liệu nhiều chiều để quan sát được tính chất cụm của tập dữ liệu đầu vào.
    - Chọn file `univariate.ipynb`, chạy tất cả chương trình để xem sự khác biệt trong việc phân bô các biến đặc trưng trong tập huấn luyện và tập kiểm thử
5.  Tại file `football_player_clustering.ipynb`, chạy tất cả chương trình để tiến hành phân cụm tập dữ liệu huấn luyện cầu thủ theo 2 phương pháp `Hierarchical Clustering` và `DBSCAN`. Xem kết quả trực quan quá trình khảo sát các tham số và tiến hành phân cụm dữ liệu.
    - So sánh các phương pháp phân cụm, xuất ra file `players_with_labels` chứa kết quả phân cụm dữ liệu cầu thủ bóng đá.
6. Tại file `football_player_classification.ipynb`, chạy tất cả chương trình để tiến hành tiền xử lý dữ liệu huấn luyện, khảo sát các tham số huấn luyện của các mô hình, tiến hành phân loại tập kiểm thử và đánh giá kết quả nhận được.

