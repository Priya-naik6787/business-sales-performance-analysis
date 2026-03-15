# business-sales-performance-analysisSuperstore Sales Data Analysis Project
📌 Project Overview

This project analyzes a Superstore retail sales dataset to identify key business insights such as sales performance, profitability, regional trends, and customer behavior.

The project demonstrates a complete Data Analyst workflow including:

Data Cleaning using Python

Data Analysis using SQL

Data Visualization using Power BI

Business insights through a final analytical report

This project simulates a real-world retail business analysis scenario.

🎯 Objectives

The main objectives of this project are:

Analyze sales and profit performance

Identify top-selling products

Understand customer segments

Evaluate regional sales performance

Identify profitable categories

Provide business recommendations

🧰 Tools & Technologies Used
Tool	Purpose
Python	Data cleaning and analysis
Pandas	Data manipulation
Matplotlib	Data visualization
SQL	Data querying and analysis
Power BI	Dashboard and visual analytics
Jupyter Notebook	Development environment
GitHub	Project version control
📂 Project Structure
Superstore_Data_Analytics_Project
│
├── data
│   └── SuperStore_Sales_Dataset.csv
│
├── python
│   └── data_cleaning_analysis.ipynb
│
├── sql
│   └── analysis_queries.sql
│
├── powerbi
│   └── superstore_dashboard.pbix
│
├── report
│   └── Superstore_Data_Analytics_Report.pdf
│
└── README.md
📊 Dataset Description

The dataset contains 5900+ retail sales transactions with information about:

Orders

Customers

Products

Sales

Profit

Shipping

Regions

Important Columns
Column	Description
Order ID	Unique order identifier
Order Date	Date of order
Ship Date	Date of shipment
Ship Mode	Shipping method
Customer Name	Customer name
Segment	Customer segment
Region	Sales region
Category	Product category
Sub-Category	Product subcategory
Sales	Total revenue
Quantity	Number of units sold
Profit	Profit generated
🧹 Data Cleaning (Python)

Data preprocessing steps included:

Handling missing values

Converting date columns

Removing duplicates

Renaming columns

Preparing dataset for analysis

Example code:

import pandas as pd

df = pd.read_csv("SuperStore_Sales_Dataset.csv")

df["Order Date"] = pd.to_datetime(df["Order Date"])
df["Ship Date"] = pd.to_datetime(df["Ship Date"])

df = df.drop_duplicates()

print(df.head())
🗄 SQL Data Analysis

SQL queries were used to analyze the dataset.

Example Queries

Total Sales

SELECT SUM(sales) AS total_sales
FROM sales;

Top 10 Products

SELECT product_name, SUM(sales) AS revenue
FROM sales
GROUP BY product_name
ORDER BY revenue DESC
LIMIT 10;

Sales by Region

SELECT region, SUM(sales)
FROM sales
GROUP BY region;
📈 Power BI Dashboard

A Power BI dashboard was created to visualize the insights.

Dashboard Includes

Total Sales KPI

Total Profit KPI

Sales by Region

Sales by Category

Top 10 Products

Monthly Sales Trend

Customer Segment Analysis

Dashboard Filters

Region

Category

Segment

Year

🔍 Key Business Insights

Some insights discovered during analysis:

The West region generated the highest revenue

Technology category contributed the highest profit

The Consumer segment accounted for the majority of sales

Certain products contributed significantly to total revenue

💡 Business Recommendations

Based on the analysis:

Focus marketing on high-performing regions

Promote top-selling product categories

Improve strategies for low-performing segments

Optimize shipping for faster delivery

📄 Project Report

A detailed data analytics report summarizing the project and insights is included.

report/Superstore_Data_Analytics_Report.pdf
🚀 How to Run the Project

Clone the repository

git clone https://github.com/yourusername/superstore-data-analysis.git

Install dependencies

pip install pandas matplotlib

Run the Python analysis notebook

jupyter notebook

Open the Power BI dashboard to explore visual insights.

👨‍💻 Author

Priya

Data Analyst | Python | SQL | Power BI | Data Visualization

⭐ If you found this project useful

Please consider starring the repository ⭐
