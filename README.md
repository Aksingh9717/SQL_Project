
# Walmart Sales Data Analysis



## Overview

This project is designed to delve into Walmart's sales data to uncover insights about top-performing branches and products, examine sales trends across different items, and analyze customer behavior. The goal is to identify opportunities to enhance and streamline sales strategies. The data for this analysis is sourced from the Kaggle Walmart Sales Forecasting Competition.

"In this competition, participants are given historical sales data for 45 Walmart stores spread across various regions. Each store has multiple departments, and the challenge involves forecasting sales for each department in every store. Additionally, the dataset includes selected holiday markdown events, which are known to impact sales but are difficult to predict in terms of which departments are influenced and the degree of impact." source


### Project Goals

The primary objective of this project is to analyze Walmart's sales data to understand the factors influencing sales performance across different branches.


### Data Details

The dataset, obtained from the Kaggle Walmart Sales Forecasting Competition, includes sales transactions from three Walmart branches located in Mandalay, Yangon, and Naypyitaw. The data comprises 17 columns and 1,000 rows.


| Column                  | Description                             | Data Type      |
| :---------------------- | :-------------------------------------- | :------------- |
| invoice_id              | Invoice of the sales made               | VARCHAR(30)    |
| branch                  | Branch at which sales were made         | VARCHAR(5)     |
| city                    | The location of the branch              | VARCHAR(30)    |
| customer_type           | The type of the customer                | VARCHAR(30)    |
| gender                  | Gender of the customer making purchase  | VARCHAR(10)    |
| product_line            | Product line of the product solf        | VARCHAR(100)   |
| unit_price              | The price of each product               | DECIMAL(10, 2) |
| quantity                | The amount of the product sold          | INT            |
| VAT                 | The amount of tax on the purchase       | FLOAT(6, 4)    |
| total                   | The total cost of the purchase          | DECIMAL(10, 2) |
| date                    | The date on which the purchase was made | DATE           |
| time                    | The time at which the purchase was made | TIMESTAMP      |
| payment_method                 | The total amount paid                   | DECIMAL(10, 2) |
| cogs                    | Cost Of Goods sold                      | DECIMAL(10, 2) |
| gross_margin_percentage | Gross margin percentage                 | FLOAT(11, 9)   |
| gross_income            | Gross Income                            | DECIMAL(10, 2) |
| rating                  | Rating                                  | FLOAT(2, 1)    |



### Analysis Overview

### Product Analysis

This analysis focuses on evaluating various product lines to determine which ones are performing well and which ones require improvements.

### Sales Analysis

This analysis aims to uncover sales trends across different products. The insights gained will help assess the effectiveness of current sales strategies and identify necessary adjustments to boost sales.

### Customer Analysis

This part of the analysis seeks to identify different customer segments, their purchasing behaviors, and the profitability associated with each segment.

### Methodology
Data Wrangling: The initial step involves examining the dataset to identify and address NULL or missing values using appropriate replacement methods.

### Create a database
Define tables and insert the data.
Identify columns with missing values. In this case, as tables are set with NOT NULL constraints, no missing values are present in our database.
#### Feature Engineering: This process involves creating new columns from existing data to gain additional insights.

#### Introduce a (time_of_day) column to categorize sales by Morning, Afternoon, and Evening, helping determine peak sales times.

#### Add a (day_name) column to record the day of the week for each transaction (e.g., Mon, Tue, Wed). This will help identify which days are busiest for each branch.
#### Create a (month_name) column to capture the month of each transaction (e.g., Jan, Feb, Mar), aiding in the analysis of monthly sales and profits.
#### Exploratory Data Analysis (EDA): 
This step involves analyzing the data to answer the key questions and objectives outlined in the project.

#### Conclusion:

#### Key Questions to Address
### General

#### 1.How many unique cities are represented in the data?

![Screenshot 2024-08-28 212334](https://github.com/user-attachments/assets/48f4d04e-c657-4118-bf6e-080a926003d6)

#### 2. In which city is each branch located?

![Screenshot 2024-08-28 213107](https://github.com/user-attachments/assets/ad7baf98-ae95-43ed-bf38-f911e0b91e08)

### Product

#### 1. How many distinct product lines are there?

![Screenshot 2024-08-28 213148](https://github.com/user-attachments/assets/41cb7278-0a7d-4a49-8aef-0cefe591e91c)


#### 2. What is the most frequently used payment method?

![Screenshot 2024-08-28 213358](https://github.com/user-attachments/assets/f2b53fb3-8832-42a3-872b-ffac3f4a16b1)


#### 3. Which product line generates the highest sales?

![Screenshot 2024-08-28 213436](https://github.com/user-attachments/assets/46acea1f-63ff-420b-8f6e-e3425ec6fc94)



#### 4. What is the total revenue by month?

![Screenshot 2024-08-28 220322](https://github.com/user-attachments/assets/18b2b5cc-3dca-4e2e-a689-e6d1882f533b)



#### 5. Which month has the highest Cost of Goods Sold (COGS)?
![Screenshot 2024-08-28 213522](https://github.com/user-attachments/assets/c74b8bda-4aaf-4037-9750-64e57a68360e)


#### 6. Which product line has the highest revenue?

![Screenshot 2024-08-28 213537](https://github.com/user-attachments/assets/fc649624-ff24-481d-8f31-05f4d5f685dd)


#### 7. Which city generates the most revenue?

![Screenshot 2024-08-28 213549](https://github.com/user-attachments/assets/f0ae971a-26e2-4673-a265-a0f6379b0587)


#### 8. Which product line has the highest VAT?

![Screenshot 2024-08-28 213603](https://github.com/user-attachments/assets/58221e7e-a614-47f9-9f63-f2471475e62c)


#### 9. What is the most popular product line among different genders?

![Screenshot 2024-08-28 213625](https://github.com/user-attachments/assets/6162aaa8-8b55-4828-9931-a850ffda4c19)


#### 10. What is the average rating for each product line?

![Screenshot 2024-08-28 215229](https://github.com/user-attachments/assets/de94826a-ceb9-45af-a797-f9d08b6365e4)


### Sales

#### 1. How many sales occur at different times of day and weekdays?

![Screenshot 2024-08-28 220452](https://github.com/user-attachments/assets/9aa48469-a1c3-40fb-bd59-d599a4c7ffb9)


#### 2. Which customer type contributes the most revenue?

![Screenshot 2024-08-28 220505](https://github.com/user-attachments/assets/ca40f390-ef11-4d46-8ced-f936c7727474)


#### 3. Which city has the highest VAT percentage?

![Screenshot 2024-08-28 220518](https://github.com/user-attachments/assets/cc4679af-ec20-4e7d-8e05-786047184f6e)


#### 4. Which customer type incurs the most VAT?

![Screenshot 2024-08-28 220531](https://github.com/user-attachments/assets/48b9a8c9-7177-416f-89cb-d56c06d558f2)



### Customer

#### 1. How many unique customer types are there?

![Screenshot 2024-08-28 220808](https://github.com/user-attachments/assets/50ffff11-9a28-44f1-bef2-b919483e5e21)


#### 2. How many different payment methods are used?

![Screenshot 2024-08-28 220820](https://github.com/user-attachments/assets/04d44681-be41-424f-8057-96df37aa151d)


#### 3. What is the most common customer type?

![Screenshot 2024-08-28 220833](https://github.com/user-attachments/assets/c23a8818-8058-4fce-970e-b71e3cdfeee0)



#### 4. What is the gender of most of the customers?

![Screenshot 2024-08-28 220850](https://github.com/user-attachments/assets/3e4fa07d-2d4a-4d05-af8c-066ba6b65284)



#### 5. What is the predominant gender of customers in each branch?

In Branch "A" ![Screenshot 2024-08-28 220901](https://github.com/user-attachments/assets/9d58ed94-5024-4f24-a756-8eac6dc9521e)

In Branch "B"![Screenshot 2024-08-28 221517](https://github.com/user-attachments/assets/09442998-664f-4227-9a8f-e196a8c6f20a)

In Branch "C" ![Screenshot 2024-08-28 221531](https://github.com/user-attachments/assets/5a2017a6-5ce8-4581-8e75-bb416076ecdf)



#### 6. At which time of day do customers give the most ratings?
![Screenshot 2024-08-28 220939](https://github.com/user-attachments/assets/c630ec99-886a-4b70-8746-80762adf7fa0)


#### 7. At which time of day do customers give the most ratings?

![Screenshot 2024-08-28 221950](https://github.com/user-attachments/assets/d60d32af-4508-45c9-80d7-05a047cdea20)


#### 9. On which day of the week are ratings highest on average?

![Screenshot 2024-08-28 222003](https://github.com/user-attachments/assets/b95db75b-78fe-405f-ad6f-d168ba218c1f)


#### 10.On which day of the week do branches receive the highest average ratings?

In Branch "A" ![Screenshot 2024-08-28 222655](https://github.com/user-attachments/assets/778ee55c-3f5a-4aec-8efa-a4e46ccb9506)
In Branch "B" ![Screenshot 2024-08-28 222707](https://github.com/user-attachments/assets/152a52d6-e5a2-4e5c-9dfa-bff1f0f53540)
In Branch "C" ![Screenshot 2024-08-28 222719](https://github.com/user-attachments/assets/1f0f1c9e-7304-4c88-bd7d-14bc86bae893)



