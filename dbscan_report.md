## Ưu điểm
- Phân cụm theo mật độ (bỏ qua các outlier)
- Tìm được các cluster non-linear
- Có 1 số điểm k thuộc bất kỳ 1 cụm nào
- K cần biết trc số cụm như k-means

```Bỏ qua noise, k làm biến dạng cluster```
## Nhược điểm
- Phải tìm đc eps (ngưỡng)
- Phù hợp với bài toán mà dữ liệu có mật độ đồng đều
## Tham số
- min_distance: k/c giữa 2 điểm đc coi là neighbor point (k/c euclide)
    + sử dụng k-distance
- min_points: số điểm neighbor point tối thiểu để tạo thành 1 cụm
    + min_points >= D + 1 >=3 (D là số chiều của tập dữ liệu). Thường chọn min_points = 2xdim (nhiễu càng nhiều thì min_points càng lớn)
- core point: 1 điểm đc coi là core point nếu có tối thiểu min_point có min_distance
## Thuật toán
- Step 1:
    + Đếm số lượng điểm neighbor point của mỗi điểm
    + Xác định các core points
- Step 2:
    + Chọn random core point (không nằm trong cụm nào cả), gán vào 1 cụm
    + Tìm xung quanh core point, nếu có core point nào là neighbor thì add vào cụm
    + Tìm tiếp xung quanh các core point trong cụm, tiếp tục mở rộng cho đến khi k còn điểm core point nào để add
- Step 3:
    + Tìm các điểm k là core point nhưng là neighbor để thêm vào cụm (thêm vào nhưng k mở rộng cụm)
- Step 4:
    + Tăng số cụm, quay lại bước 2