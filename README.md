### Supermarket Sales Data Analysis


## About
This project aims to delve into the sales data of a supermarket chain to gain insights into top-performing branches, popular products, sales trends, and customer behavior. The dataset used for this analysis comprises sales transactions from multiple branches of the supermarket chain.



## Purposes Of The Project
The primary objective of this project is to understand the factors influencing sales across different branches of the supermarket chain and to identify opportunities for improving and optimizing sales strategies.



## About Data
The dataset contains sales transactions from multiple branches of the supermarket chain. Each transaction includes information such as invoice ID, branch location, customer type, product details, unit price, quantity sold, total amount, date, time, payment method, cost of goods sold (COGS), gross margin percentage, gross income, and customer rating.
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




## Analysis List
# Product Analysis
Conduct analysis to understand the various product categories, identify best-selling products, and pinpoint areas for product line improvement.
# Sales Analysis
Explore sales trends over time, analyze revenue by product category and branch location, and evaluate the effectiveness of different sales strategies.
# Customer Analysis
Identify customer segments, analyze purchase patterns, and assess the profitability of each customer segment.
## Approach Used
Data Wrangling
> Ensure data cleanliness by handling missing values and 
 filtering out irrelevant information.
> Prepare the dataset for analysis by creating a structured 
  database and defining appropriate data types for each 
  column.
## Feature Engineering
Generate new features from existing data to provide additional insights, such as time of day for sales and day of the week for transactions.
## Exploratory Data Analysis (EDA)
Utilize exploratory data analysis techniques to answer key business questions and uncover actionable insights from the data.
## ConclusionSummarize
findings from the analysis and provide recommendations for improving sales performance and customer satisfaction.
Business Questions To Answer
# Generic Questions
1.Determine the number of unique branches and their locations.

2.Identify the most common payment methods used by customers.
# Product Analysis
1.Determine the most popular product categories.

2.Analyze revenue by product category and identify the top-performing categories.

3.Investigate seasonal variations in sales and profitability.
# Sales Analysis
1.Analyze sales trends over time and identify peak sales periods.

2.Assess revenue contribution from different branches and regions.

3.Investigate the impact of promotions and discounts on sales performance.
# Customer Analysis
1.Identify the most valuable customer segments based on revenue contribution.

2.Analyze customer purchasing behavior and preferences.

Assess customer satisfaction levels and identify areas for improvement.
# Code
-- Create database
CREATE DATABASE IF NOT EXISTS supermarketsales;

-- Create table

CREATE TABLE IF NOT EXISTS sales(
invoice_id VARCHAR(30) NOT NULL PRIMARY KEY,
 
    branch VARCHAR(5) NOT NULL,
    
    city VARCHAR(30) NOT NULL,
    
    customer_type VARCHAR(30) NOT NULL,
    
    gender VARCHAR(30) NOT NULL,
    
    product_line VARCHAR(100) NOT NULL,
    
    unit_price DECIMAL(10,2) NOT NULL,
    
    quantity INT NOT NULL,
    
    tax_pct FLOAT(6,4) NOT NULL,
    
    total DECIMAL(12, 4) NOT NULL,
    
    date DATETIME NOT NULL,
    
    time TIME NOT NULL,
    
    payment VARCHAR(15) NOT NULL,
    
    cogs DECIMAL(10,2) NOT NULL,
    
    gross_margin_pct FLOAT(11,9),
    
    gross_income DECIMAL(12, 4),
    
    rating FLOAT(2, 1)
    );


For SQL queries and further analysis, refer to the SQL_queries.sql file in the project repository.


This adapted overview provides a framework for analyzing supermarket sales data, covering key aspects such as product analysis, sales trends, and customer behavior. If you have any specific questions or need assistance with further details, feel free to ask!






# Supermarket-sales
