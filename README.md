# Project-Applied_Data_Science
## Đồ án môn Khoa học Dữ liệu và Ứng Dụng
### GVHD: Trần Trung Kiên
### Nhóm: 12
### DANH SÁCH THÀNH VIÊN:
  1. 1712667 - Lê Hữu Phúc - PhucLe2303
  2. 18120167 - Nguyễn Viết Dũng - kaiser1038
  3. 18120579 - Đặng Minh Thọ - MinhTho-162
  4. 18120584 - Phạm Đình Thục - pdthuc
 
### KẾ HOẠCH THỰC HÀNH:
- Link google sheets: https://docs.google.com/spreadsheets/d/1kb0j4sLcvcjz4rnoe6WSbI112LpuAlqCxAsfA99TE5E/edit?usp=sharing

### LINK GOOGLE COLAB
- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pdthuc/Project-Applied_Data_Science/blob/main/Group12_kaggle_recruit_restaurant.ipynb)

- **Tên cuộc thi:** Recruit Restaurant Visitor Forecasting
- **Mô tả bài toán:** 
    - Bài toán dự đoán **số lượng khách hàng** sẽ đến **01 nhà hàng** vào **01 ngày bất kỳ** trong tương lai. Việc dự đoán sẽ dựa vào các thông tin về vị trí (kinh độ, vĩ độ) của nhà hàng, các ngày lễ trong năm, thông tin dự báo thời tiết ngày hôm đó và dữ liệu đặt chỗ thông qua trang web đặt chỗ của nhà hàng và dữ liệu khách đã đến trong cơ sở dữ liệu của nhà hàng.
    - **Input**: là mã của nhà hàng (`air_store_id`) và ngày cần dự đoán (`visit_date`).
    - **Output**: Số lượng khách (`visitors`) sẽ đến nhà hàng.
- **Prize:** $ 25000
- **Participants:** 2148 teams
- **Link Kaggle:** https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting

- **Solution:**
  - Trong đồ án này, nhóm đã tìm hiểu và cài đặt lại phương pháp nằm trong top 10 Private Leaderboard.
  - Xếp hạng solution: Top 8 Private Leaderboard với `score` = 0.50775
  - Tác giả: MaxHalford 
  - Link Solution: https://github.com/MaxHalford/kaggle-recruit-restaurant

Dữ liệu đến từ hai trang web riêng biệt: 
  - Hot Pepper Gourmet (hpg): tại đây người dùng có thể tìm kiếm nhà hàng và đặt chỗ trực tuyến 
  - AirREGI / Restaurant Board (air): hệ thống kiểm soát đặt chỗ và tính tiền
  
Được thu thập từ năm 2016 đến tháng 4 năm 2017 
- AIR: 829 restaurants 
- HPG: 4690 restaurants

Dữ liệu thu thập bao gồm các thông tin liên quan đến nhà hàng (id, latitude, longitude, ...), các thông tin về số lượng khách đặt chỗ tại các nhà hàng và các thông tin liên quan đến thời tiết, ngày lễ.

Để hoàn thành đồ án này, nhóm mình đã tham khảo những tài liệu sau:
1. https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting
2. https://github.com/MaxHalford/kaggle-recruit-restaurant
3. https://www.statisticshowto.com/probability-and-statistics/z-score/
4. https://www.mathsisfun.com/data/confidence-interval-calculator.html
5. https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.ewm.html
6. https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMRegressor.html
7.  https://lightgbm.readthedocs.io/en/latest/
8. https://miai.vn/2021/01/18/k-fold-cross-validation-tuyet-chieu-train-khi-it-du-lieu/
9. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.KFold.html

Và nhóm xin gửi lời cảm ơn đặc biệt đến https://stackoverflow.com/ vì đã hỗ trợ nhóm trong quá trình làm đồ án này. :">
