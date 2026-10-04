

# 🛒 Zepto Sales Data Analysis

> Exploratory Data Analysis of 220K+ Zepto sales transactions using Python, Pandas, Matplotlib, and Seaborn.

## 📌 Project Overview

This project performs an exploratory data analysis of Zepto sales data to understand sales performance, product performance, city-wise sales, product categories, monthly sales trends, and delivery efficiency.

The project follows a complete data analysis workflow:

**Data Loading → Data Exploration → Data Cleaning → Data Analysis → Data Visualization → Business Insights**

The analysis was developed using Python in Google Colab.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Analyze overall sales performance
- Identify the top-performing products
- Compare sales performance across cities
- Analyze sales by product category
- Identify monthly sales trends
- Compare delivery efficiency across cities
- Analyze transaction amounts
- Understand the relationship between quantity sold and transaction value
- Present findings through meaningful visualizations

---

## 📂 Project Structure

```text
zepto-sales-data-analysis/
│
├── 📁 dataset/
│   ├── zepto_sales.csv
│   └── zepto_products.csv
│
├── 📓 PYTHON_PROJECT.ipynb
│
└── 📄 README.md

📊 Dataset Description

The project uses two related datasets.

1. zepto_sales.csv

This dataset contains individual sales transactions.

Column	Description
order_id	Unique identifier for each order
order_date	Date and time of the order
product_id	Identifier for the product sold
quantity	Number of units sold
city	City where the order was placed
delivery_status	Delivery status of the order
customer_id	Unique identifier for the customer
delivery_time_mins	Delivery time in minutes
total_amount	Total amount of the transaction
2. zepto_products.csv

This dataset contains product information.

Column	Description
product_id	Unique identifier for the product
product_name	Name of the product
category	Product category
base_price	Base price of the product

The two datasets are connected through the product_id column.

🛠️ Technologies Used
Python
Pandas
Matplotlib
Seaborn
Google Colab / Jupyter Notebook

🔍 Data Analysis Workflow
1. Data Loading & Initial Exploration

The datasets were loaded using Pandas and explored using:

info()
describe()
shape
head()
tail()

The original sales dataset contains 220,220 records and 9 columns, while the product dataset contains 38 products and 4 columns.

2. Data Cleaning

The sales data was cleaned by:

Checking for missing values
Removing records with missing city and delivery_status
Filling missing delivery_time_mins values using the mean
Identifying and removing duplicate records
Converting order_date to datetime format

A total of 216 duplicate records were removed, leaving 217,806 records after cleaning.

3. Exploratory Data Analysis

The analysis covers:

Summary statistics
Top products by sales
Total sales by city
Average delivery time by city
Monthly sales trends
Sales by product category
4. Data Visualization

The project contains 9 visualizations:

📈 Monthly Sales Trend
🏙️ Total Sales by City
🥧 Sales by Product Category
🚚 Distribution of Delivery Times
📦 Quantity vs Total Amount
🚛 Delivery Status Distribution
⏱️ Delivery Time by City
🏆 Top 5 Products by Quantity Sold
🔥 Sales by City and Month
💡 Key Insights
🏙️ Top Performing City

Mumbai recorded the highest total sales at approximately:

₹23.06 million

It was followed by Bangalore and Delhi.

🛍️ Top Performing Category

Personal Care was the highest-performing product category with approximately:

₹23.40 million in sales

🏆 Top Products by Sales

The top 5 products by total sales amount were:

Rank	Product	Sales
1	Handwash	₹11.66M
2	Paneer 200g	₹7.91M
3	Toothpaste	₹6.17M
4	Detergent 1kg	₹4.80M
5	Toilet Paper	₹4.72M
📅 Monthly Sales

Sales remained relatively consistent throughout 2024.

December 2024 recorded the highest monthly sales at approximately:

₹5.69 million

🚚 Delivery Efficiency

The average delivery time across the analyzed cities was approximately 26 minutes.

Hyderabad: ~25.91 minutes
Mumbai: ~25.98 minutes
Bangalore: ~26.02 minutes
Delhi: ~26.04 minutes
Pune: ~26.04 minutes
Chennai: ~26.06 minutes
Kolkata: ~26.09 minutes
Ahmedabad: ~26.17 minutes

The difference between cities was relatively small, indicating fairly consistent delivery times.

💰 Transaction Analysis
Minimum transaction amount: ₹23.25
Maximum transaction amount: ₹2,656.85
Average transaction amount: ₹302.32
📈 Business Questions Answered

This project answers questions such as:

Which city generates the highest sales?
Which product category performs best?
Which products generate the highest sales?
What is the monthly sales trend?
Which cities have the lowest and highest average delivery times?
What is the average transaction value?
How does quantity relate to total transaction amount?
How are orders distributed by delivery status?
▶️ How to Run the Project
⭐ Recommended: Google Colab

This project was developed in Google Colab.

You can run the notebook without changing the existing file paths.

Step 1 — Open the Notebook

Open:

PYTHON_PROJECT.ipynb

in Google Colab.

Step 2 — Download the Datasets

From the dataset folder in this repository, download:

zepto_sales.csv
zepto_products.csv
Step 3 — Upload the Datasets to Colab

In Google Colab:

Open the Files panel on the left.
Click the Upload button.
Upload both CSV files.
Make sure both files appear directly inside /content/.

The Colab Files panel should look like:

/content/
│
├── zepto_sales.csv
└── zepto_products.csv
Step 4 — Run the Notebook

Run the notebook from the beginning using:

Runtime → Run all
📌 Important

The notebook currently uses:

df_sales = pd.read_csv("/content/zepto_sales.csv")
df_products = pd.read_csv("/content/zepto_products.csv")

Therefore, you do not need to modify the file paths.

Simply upload the two datasets directly into the Colab Files section and run the notebook.

📦 Required Libraries

The project uses:

pandas
matplotlib
seaborn

If necessary, install them using:

pip install pandas matplotlib seaborn
🎓 Skills Demonstrated

This project demonstrates practical experience with:

Python
Pandas
Data Cleaning
Data Preprocessing
Exploratory Data Analysis (EDA)
Data Aggregation
GroupBy Operations
Datetime Analysis
Data Visualization
Matplotlib
Seaborn
Business Insight Generation
Data Storytelling
📌 Conclusion

This project demonstrates how raw sales transaction data can be transformed into meaningful business insights using Python.

The analysis identified high-performing cities, products, and categories while also examining monthly sales trends, transaction values, and delivery efficiency.

The findings provide a useful overview of sales and operational performance and demonstrate the practical application of Python-based data analysis and visualization techniques.

👨‍💻 Author

Sujal Choudhary

Python Data Analysis Project
