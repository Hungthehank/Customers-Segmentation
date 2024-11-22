# Customers-Segmentation
Use Python Programming for customers segmentation, create a campaign to reward loyal customers, and attract potential customers to buy more often.

- Ngữ cảnh:
  
Công ty SuperStore là một công ty bán lẻ trên toàn cầu - Global. Nên công ty có rất nhiều khách hàng.
Nhân dịp giáng sinh và năm mới, phòng Marketing muốn chạy các chiến dịch marketing để tri ân khách hàng đã ủng hộ công ty suốt thời gian qua. Cũng như khai thác các khách có tiềm năng trở thành khách hàng trung thành.
    
Tuy nhiên phòng Marketing vẫn chưa phân nhóm cho từng khách hàng của năm nay được vì tập dữ liệu quá lớn nên không thể xử lý bằng tay như các năm trước, nên nhờ Phòng Phân tích dữ liệu hỗ trợ triển khai một bài toán phân loại phân khúc của từng khách hàng để triển khai từng chương trình marketing phù hợp với từng nhóm khách hàng.

Giám đốc Marketing cũng có đề xuất phương án sử dụng mô hình RFM, tuy nhiên trước đây khi quy mô công ty nhỏ, team có thể tự tính và phân loại bằng excel. Hiện tại lượng data quá lớn nên mong muốn Phòng dữ liệu xây dựng luồng triển khai đánh giá Segmentation thông qua lập trình Python.
    

- Hướng tiếp cận đề xuất:
    
    1. Chuẩn bị tập dữ liệu phù hợp với mô hình RFM.
    
    2. Xác định cách tính và tính điểm R, F, M của từng khách hàng.
    
    3. Đưa ra cách tính với tính điểm tương ứng với thang điểm từ 1 đến 5.
    
    Gợi ý: sử dụng phương pháp ngũ phân vị - quintile của Thống kê.
    
    4. Dựa vào bảng phân loại để gom nhóm cho từng khách hàng
    
    5. Visualize số lượng của các tập segment với các chiều dữ liệu - Dimension
    
    6. Phân tích hiện trạng của công ty và đưa ra gợi ý cho team Marketing
    
### Segmentation File:
    
![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/a681ec0b-9a6c-4046-9965-308942886954/876a5089-d9a2-441e-962f-cc97e4a1dbac/image.png)
    
### 1. Dataframe
![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/a681ec0b-9a6c-4046-9965-308942886954/5a386a1b-184c-4e1a-a373-a24dd7264596/image.png)
    
![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/a681ec0b-9a6c-4046-9965-308942886954/a1f91e9e-3f4a-467c-ba97-2baa31a791b5/image.png)
    
Có 541909 dòng, 8 cột
    
### 2. EDA
    
    
### 3. Tính điểm, phân loại
    
    
### 4. Visualization
        
    
### 5. Recommendation
    
    - Sau khi segment: Nhóm Hibernating customers, Champions chiếm số lượng vượt trội hơn các nhóm còn lại, tuy nhiên nhóm Hibernating chỉ mang lại 3.8 doanh số, chúng ta không cần quá lo lắng.
    - Tập trung công việc **tri ân** vào nhóm: **Champions, Loyal.**
    - Tập trung công việc lôi kéo khách hàng tiềm năng: New Customers, Potential Loyalist.
