Retail Orders Data Analysis Project
This project provides analysis on retail order data using Python for data processing and SQL for querying. The analysis helps derive insights into product performance, sales trends, and profit growth across various categories.

Project Overview
The project involves the following steps:

Data Extraction: Extract the retail order dataset from a Kaggle zip file.
Data Processing: Load the data, handle null values, derive new columns (discount, sale price, profit), and perform data cleaning.
Data Storage: Store the processed data into a SQL Server database.
Data Analysis: Perform SQL queries to derive business insights like top-performing products, month-over-month sales growth, and highest sales by category.
Project Structure
Python Script (retail_orders_analysis.py)
Data Extraction: Downloads and extracts the retail orders dataset from Kaggle.
Data Cleaning and Transformation:
Handles null values.
Converts column names to lowercase and replaces spaces with underscores.
Derives new columns for discount, sale price, and profit.
Converts order_date to a datetime format.
Drops unnecessary columns such as list_price, cost_price, and discount_percent.
Data Loading: The processed data is loaded into a SQL Server database for further querying and analysis.
SQL Scripts (retail_orders_analysis.sql)
Top 10 Highest Revenue Generating Products: Query to find the top 10 products with the highest sales.
Top 5 Highest Selling Products by Region: Query to find the top 5 products in each region based on sales.
Month-over-Month Growth Comparison: Query to compare month-over-month sales for 2022 vs 2023.
Highest Sales by Category: Query to determine which month had the highest sales for each category.
Subcategory with Highest Growth in Profit: Query to find the subcategory with the highest growth in profit in 2023 compared to 2022.
How to Run the Project
Prerequisites
Python 3.x
Pandas
SQLAlchemy
SQL Server
Kaggle API
Steps to Run
Clone the repository.

bash
Copy code
git clone <repo-url>
cd <repo-directory>
Install necessary Python libraries:

bash
Copy code
pip install pandas sqlalchemy kaggle
Download the dataset from Kaggle using the Kaggle API:

bash
Copy code
kaggle datasets download ankitbansal06/retail-orders -f orders.csv
Run the Python script to process and load data into SQL Server:

bash
Copy code
python retail_orders_analysis.py
Execute the SQL queries in retail_orders_analysis.sql on the SQL Server to perform data analysis.

SQL Server Setup
Ensure that SQL Server is running on your local machine.
Update the connection string in the Python script with the correct server name and database credentials.
Results and Insights
This project provides various insights such as:

The highest revenue-generating products.
Regional product performance.
Monthly sales growth.
Sales trends by category.
Growth analysis by subcategory.
License
This project is licensed under the MIT License.
