# Walmart Sales Data Analysis


## Project Overview

This project is dedicated to the comprehensive exploration of Walmart sales data with the objective of gaining insights into the performance of distinct branches and products. The analysis aims to discern patterns in sales trends across various product categories and delve into customer behavior. Through this exploration, the project seeks to provide valuable insights that contribute to the refinement and improvement of sales strategies within the Walmart retail framework. The dataset has been obtained from the [Kaggle Walmart Sales Forecasting Competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting).

## Purposes Of The Project

The major aim of thie project is to gain insight into the sales data of Walmart to understand the different factors that affect sales of the different branches.

## About the Data

The dataset was obtained from the [Kaggle Walmart Sales Forecasting Competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting). This dataset contains sales transactions from three different branches of Walmart namely Mandalay, Yangon and Naypyitaw. The data contains 17 columns and 1000 rows:

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


### Analysis List

1. Product Analysis

> Conduct analysis on the data to understand the different product lines, the products lines performing best and the product lines that need to be improved.

2. Sales Analysis

> This analysis aims to answer the question of the sales trends of product. The result of this can help use measure the effectiveness of each sales strategy the business applies and what modificatoins are needed to gain more sales.

3. Customer Analysis

> This analysis aims to uncover the different customers segments, purchase trends and the profitability of each customer segment.


## Approach Used

1. **Data Wrangling:** In the initial phase, the data undergoes an inspection to identify and address instances of **Null** values and missing data. Robust data replacement methodologies are then employed to substitute missing or **Null** values, ensuring the integrity and completeness of the dataset. 

> 1. Build a database
> 2. Create table and insert the table columns as per the dataset.
> 3. Importing data to the created table

2. **Feature Engineering:** In this step we will  generate some new features or columns from the existing ones.

> 1. We will add a new column named `time_of_day` to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.

> 2. We will add a new column named `dayname` that would contain the days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri, Sat, Sun). This will help answer the question on which day od the week each branch is busiest.

> 3. We will add a new column named `month` that would contain the months of the year on which the given transaction took place (Jan, Feb, Mar,...). Thsi will help to determine which month of the year has the most sales.

3. **Exploratory Data Analysis (EDA):** An exploratory data analysis is done to answer various questions regarding the Product Lines, Sales, and Customers which is the aim of this project.
