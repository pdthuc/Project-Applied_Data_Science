# Project-Applied_Data_Science
## Đồ án môn Khoa học Dữ liệu và Ứng Dụng
### GVHD: Trần Trung Kiên
### Nhóm: 12
### DANH SÁCH THÀNH VIÊN:
  1. 1712667 - Lê Hữu Phúc - PhucLe2303
  2. 18120167 - Nguyễn Viết Dũng - kaiser1038
  3. 18120579 - Đặng Minh Thọ - MinhTho-162
  4. 18120584 - Phạm Đình Thục - phamdinhthuc020100
## 1. CHỌN ĐỀ TÀI
- Tên cuộc thi: **`Recruit Restaurant Visitor Forecasting`**
- Mô tả tổng quan: Dự đoán nhà hàng sẽ nhận được bao nhiêu khách trong tương lai
- Link cuộc thi: https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting
- Link **`TOP 8`** Solution: https://github.com/MaxHalford/kaggle-recruit-restaurant

## 2. GIỚI THIỆU ĐỀ TÀI
  *(Đã cập nhật slide giới thiệu đề tài)*
- Đặt vấn đề
- Tổng quan cuộc thi
- Giới thiệu Data
- Giới thiệu Solution 

## 3. KHÁM PHÁ DỮ LIỆU
*(Đã cập nhật khám phá dữ liệu)*

- Trong file air_visit_data.csv liên quan về dữ liệu khách theo ngày:
Trong file biểu diễn dữ liệu theo ngày (những ngày không có khách sẽ không được thu thập)
-> Ta cần phải lấy mẫu theo ngày thay vì theo lượt truy cập. Do đó, những ngày không có khách thì lượt truy cập sẽ là 0. Có ích cho việc tính toán luân phiên dựa vào thời gian
![image](https://user-images.githubusercontent.com/76215500/142220439-675dfab0-00d2-4353-96a5-12d737bc183f.png)

- Trong file date_info.csv liên quan đến dữ liệu các ngày lễ
Ta thêm hai tính năng cho biết ngày hôm trước và ngày hôm sau là ngày lễ hay không?
-> Điều này giúp ta biết được ngày đó là ngày lễ đơn hay là kỳ nghỉ lễ dài ngày
![image](https://user-images.githubusercontent.com/76215500/142220501-b5a79b33-66be-4161-83f9-e810855d3897.png)

- Đối với thông tin của nhà hàng ở đây chúng ta sử dụng phiên bản xử lý trước thay vì phiên bản hiện tại của cuộc thi (vì nó chứa dữ liệu quan trong của các trạm quan sát thời tiết). Bạn có thể truy cập dữ liệu này ở đây.
Dữ liệu này chứa thêm các đặc trưng như: station_id (id của các trạm gần nhà hàng nhất), station_latitude (vĩ độ của trạm), station_longitude (kinh độ),…
![image](https://user-images.githubusercontent.com/76215500/142220522-c1ff990d-7576-4091-a9b6-b74341aad200.png)

- Tiếp theo chúng ta xử lý tập test, ở đây chúng ta sử dụng file sample_submission.csv để lấy dữ liệu test. Ta trích xuất id của nhà hàng và ngày tháng từ cột id. Vì id trong sample là chuỗi gồm id + visit_date
-> Ta cần tách ra id riêng và visit_date riêng
-   Cột test_number nhằm để các kết quả dự đoán (bài nộp) được sắp xếp theo đúng thứ tự
![image](https://user-images.githubusercontent.com/76215500/142220544-c3f7beea-558b-4e30-83e7-d871c81f91ce.png)

- Sau khi hoàn thành trích xuất 2 tập train và test theo cùng 1 format. Hợp nhất train set và test set là một ý tưởng hay để trích xuất các tính năng.
Nhờ vào lượng dữ liệu hơn so với phiên bản chính thức của Kaggle. Việc hợp nhất test set và train set sẽ cho ta bộ dữ liệu tốt nhất có thể trong khâu chuẩn bị dữ liệu với thông tin lịch và thông tin cửa hàng đã trích xuất trước đó..
![image](https://user-images.githubusercontent.com/76215500/142220560-e7e548ad-2c39-455c-8fff-8ea7adc9c229.png)

- Chuẩn bị dữ liệu thời tiết – bởi được lưu trữ ở nhiều file ứng với mỗi trạm thời tiết. Nên dữ liệu này  có nhiều phần thiếu (do tính chất không cần thiết  của thời tiết khu vực tại từng trạm hoặc lí do khác ).
![image](https://user-images.githubusercontent.com/76215500/142220607-fa79503f-fb53-4d77-970b-f87cf17c6724.png)

- Ta sẽ sử dụng các dữ liệu về lượng mưa và nhiệt độ (lượt bỏ các giá trị khác).
Tiến hành xử lý các giá trị bị thiếu bằng cách thay thế chúng bằng giá trị trung bình hàng ngày trên toàn cầu
![image](https://user-images.githubusercontent.com/76215500/142220641-fd0291b0-7590-4a95-9412-a327d493486b.png)

- Sau quá trình khám phá dữ liệu, ta thu được bộ dữ liệu như sau:
![image](https://user-images.githubusercontent.com/76215500/142220663-40b385ea-e981-465f-a7a9-be159b420fe3.png)

## 4. TIỀN XỬ LÝ

## 5. CHIA TẬP DỮ LIỆU

## 6. XÂY DỰNG MÔ HÌNH

## 7. ĐÁNH GIÁ MÔ HÌNH



