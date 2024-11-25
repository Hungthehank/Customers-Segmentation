# Customers-Segmentation
Use Python Programming for customers segmentation, create a campaign to reward loyal customers, and attract potential customers to buy more often.

- Link drive contain: Ecommerce Retail dataset, Segmentation file, code, Recommendation.
  https://drive.google.com/drive/folders/1NjvF-VSmQH72BBrkLzCy1lwvoBm_8BoQ?usp=drive_link
  
- Context:
  
SuperStore Company is a global retail company - Global, the company has lots of customers.
On the occasion of Christmas and New Year, the Marketing department wants to run marketing campaigns to thank customers who have supported the company over the past time, as well as exploit customers with the potential to become loyal customers.
    
However, the Marketing Department has not yet been able to segment each customer this year because the data set is too large to be processed manually like previous years. Therefore, the Data Analysis Department is asked to support the implementation of a segmentation problem for each customer to implement each marketing program suitable for each customer group.

The Marketing Director also proposed using the RFM model, but in the past, when the company was small, the team could calculate and classify it themselves using Excel. Currently, the amount of data is too large, so the Data Department wants to build a flow to evaluate Segmentation through Python programming.
    
## Approach

1. Prepare the data set to fit the RFM model.
2. Determine how to calculate and score R, F, M for each customer.
3. Give a calculation with a score corresponding to a scale of 1 to 5.
4. Use the classification table to group each customer.
5. Visualize the number of segment sets with data dimensions - Dimension.
6. Analyze the current situation of the company and give suggestions to the Marketing team.
    
## Segmentation File:
![image](https://github.com/user-attachments/assets/9a5ab0de-06d9-4e8b-8d22-6d76e90915c7)
![image](https://github.com/user-attachments/assets/24739124-67a2-46cc-9c78-5da3ea367072)

## 1. Dataframe
![image](https://github.com/user-attachments/assets/d428476a-9e44-4f04-a9e9-3d51a8deac2a)
![image](https://github.com/user-attachments/assets/4a81cfaf-8935-432d-ae7f-48b7a1ea6c2b)

There are 541909 rows, 8 columns

Country distribution

![image](https://github.com/user-attachments/assets/7b561912-9a8e-4f52-9b36-02239d3fa8cf)
![image](https://github.com/user-attachments/assets/b21e8f4b-6c71-409c-8cbc-5342c7ba1a07)
 
## 2. EDA
### Duplicates
![image](https://github.com/user-attachments/assets/76599588-de16-4641-befa-156cb1b4a60e)

### Delete blank data in customerID column
![image](https://github.com/user-attachments/assets/7a3e0392-92e1-43a9-b1a8-f80351d27bee)
![image](https://github.com/user-attachments/assets/57ec9218-a070-4d01-8a3d-8a0c6b4d8adc)

### Change datatype and add column year-week
![image](https://github.com/user-attachments/assets/1c24f4a5-e175-4616-99f4-b81930339cf0)

### filter united kingdom, unit_price và quantity > 0
![image](https://github.com/user-attachments/assets/e0c21f46-c705-424e-a782-41833bc5873f)
![image](https://github.com/user-attachments/assets/75e10d9c-fa22-4ed9-b7a6-f1747953db24)
![image](https://github.com/user-attachments/assets/fc1d6f52-b2c5-4dd1-aca7-70b639813a0e)
![image](https://github.com/user-attachments/assets/6681113f-ab61-4ae5-b218-43a9d85edd7c)

## 3. Scoring, segmentation

### Scoring

#### Scoring for Recency
![image](https://github.com/user-attachments/assets/767977fc-491b-4e47-b295-e1c6ea78b4a8)
![image](https://github.com/user-attachments/assets/46ee58a1-f0c6-48f6-b57f-3751d9e51323)

#### Scoring for Frequency
![image](https://github.com/user-attachments/assets/8f04dee1-a77c-4bd4-ac6b-902328d9f337)
![image](https://github.com/user-attachments/assets/8af5c23e-c4f0-4f9d-9d1e-3875f2778636)

#### Scoring for Monetary
![image](https://github.com/user-attachments/assets/6e1bf1c6-107d-4e7a-8729-51eda0f44329)
![image](https://github.com/user-attachments/assets/d744622b-d5a6-4e1b-b6c4-0b05d8ab9e28)

### Segmentation

#### Merge points to segment
![image](https://github.com/user-attachments/assets/971705be-61fe-4cb0-bec4-15f9ca2b89c7)
![image](https://github.com/user-attachments/assets/4088860e-1233-4f1d-997e-d2357e455621)

####  Transform seg table and segment
![image](https://github.com/user-attachments/assets/54602664-eec5-489e-9110-f388c78ef81b)
![image](https://github.com/user-attachments/assets/a0bbc1f2-3e75-485c-b9d4-725fd696c552)
![image](https://github.com/user-attachments/assets/15676e58-2581-4c1d-9ce3-390df77bbba7)

## 4. Visualization

### Distribution of Recency, Frequency, Monetary
![image](https://github.com/user-attachments/assets/ceabd4cc-d714-458d-b659-d25fc4c40f4f)
![image](https://github.com/user-attachments/assets/25997c56-f0cd-40c7-a557-97eece02d58e)
![image](https://github.com/user-attachments/assets/bfeb43bf-4011-4e5b-8b7e-7baa2931c8f9)
![image](https://github.com/user-attachments/assets/f3bcc345-b48e-46f1-b345-f8597a6ad1fb)
The distribution of scores in the 3 criteria (Recency, Frequency, Monetary) does not differ much.

### Customer distribution of segmentation
![image](https://github.com/user-attachments/assets/35c42883-cf5b-495b-b9fa-4bcf1095d5d5)
![image](https://github.com/user-attachments/assets/db035b94-26f0-4e40-b99a-118518f4d9e4)

### Segment by customer, segmet by total sales
![image](https://github.com/user-attachments/assets/2a93a231-3417-413a-a036-583e47a5cf3f)
![image](https://github.com/user-attachments/assets/e27a9ac7-db6f-4e8b-8714-9ddf4d305b8a)

![image](https://github.com/user-attachments/assets/6299cb45-64b5-426b-82d9-104a8933f381)
![image](https://github.com/user-attachments/assets/c5932807-9ea0-4231-bdac-88ddb2c64c4c)

![image](https://github.com/user-attachments/assets/e5461f6f-67e9-46fc-a0c9-738b428e518a)
![image](https://github.com/user-attachments/assets/2145eccb-d859-4b4a-8246-5b4c81618efd)

## 5. Recommendation
- After segmentation: The Hibernating customers and Champions groups account for a larger number of consumers than the other groups. However, the Hibernating group only accounts for **3.8%** of total revenue, much less than the revenue from the Champions and Loyal customer groups (**59.5%** and **10.8%** respectively). We don't need to worry much.
- Focus gratitude work on groups: **Champions, Loyal**.
- Focus on attracting potential customers: **New Customers, Potential Loyalist**.

