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

#### Run with Visual Studio Code

1. Clone the repo
   ```sh
   git clone https://github.com/tiennhat306/Clustering-Player-Market.git
    ```
2. Chạy các file `crawl_data.ipynb` sau đó `craw_detail.ipynb` trong thư mục gốc để thu thập dữ liệu.
3. Chạy file `clean_data.ipynb` để tiến hành làm sạch dữ liệu: sửa lỗi định dạng, xóa dữ liệu bị thiếu. Xem cách xử lý và trực quan hoá sự thay đổi của phân bố dữ liệu trước và sau xử lý.
3. Tại file `univariate_data_visualization.ipynb`, chạy tất cả chương trình để xem các thống kê mô tả trực quan về dữ liệu đơn biến đối với một vài biến quan trọng.
4. Tại file `variate_data_visualization.ipynb`, chạy tất cả chương trình để xem các mối quan hệ tiềm ẩn giữa các biến trong tập dữ liệu. Hay xem biểu đồ trực quan hoá không gian dữ liệu nhiều chiều để quan sát được tính chất cụm của tập dữ liệu đầu vào.
