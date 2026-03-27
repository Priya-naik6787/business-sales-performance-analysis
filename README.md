# business-sales-performance using superstore data

📈 Business Sales Performance Analysis

📌 Problem Statement

Businesses need data-driven insights to track performance and improve profitability. This project analyzes sales data to evaluate trends, identify growth opportunities, and optimize decision-making.

🎯 Objectives

- Analyze revenue trends over time
- Identify top-performing products and regions
- Evaluate factors affecting sales performance

🛠 Tools & Technologies

- SQL (Data Querying & Aggregation)
- Python (Pandas for Data Analysis)
- Power BI (Interactive Dashboards)

📊 Key Insights

- Certain product categories contributed to over 50% of total revenue
- Seasonal trends showed peak sales during specific months
- Regional analysis revealed top-performing locations driving business growth
- Discounts and offers had a direct impact on sales volume

📈 Dashboard

(screenshot.jpg)

📁 Project Structure

- "sales_data.csv" – Dataset
- "queries.sql" – SQL queries
- "analysis.ipynb" – Python analysis
- "dashboard.pbix" – Power BI dashboard

🚀 Conclusion

This project provides actionable insights to improve sales strategies, optimize product offerings, and enhance overall business performance.
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
