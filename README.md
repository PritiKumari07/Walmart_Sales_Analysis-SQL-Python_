# Walmart Data Analysis: End-to-End SQL + Python Project 

## Project Overview

![Project Pipeline](https://github.com/najirh/Walmart_SQL_Python/blob/main/walmart_project-piplelines.png)


This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. We utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve key business questions.

---

Project Steps

1. Set Up the Environment

Tools Used: Visual Studio Code (VS Code), Python, SQL (MySQL )
Goal: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.

2. Set Up Kaggle API

API Setup: Obtained Kaggle API token from Kaggle by navigating through profile settings and downloading the JSON file.

Configure Kaggle:

Placed the downloaded kaggle.json file in the local .kaggle folder.
Used the command kaggle datasets download -d <dataset-path> to pull datasets directly into the project.

3. Download Walmart Sales Data

Data Source: Used the Kaggle API to download the Walmart sales datasets from Kaggle.

4. Install Required Libraries and Load Data

Libraries: Installed necessary Python libraries using:
pip install pandas numpy sqlalchemy 
Loading Data: Converted the data into a Pandas DataFrame for initial analysis and transformations.

5. Explore the Data

Goal: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.

Analysis: Used functions like .info(), .columns() and .head() to get a quick overview of the data structure and statistics.

6. Data Cleaning

Remove Duplicates: Identified and removed duplicate entries to avoid skewed results.
Handle Missing Values: Dropped rows or columns with missing values.
Fix Data Types: Ensured all columns have consistent data types (e.g., dates as datetime, prices as float).
Currency Formatting: Used .replace() to handle and format currency values for analysis.


7. Feature Engineering

Create New Columns: Calculated the Total Amount for each transaction by multiplying unit_price by quantity and adding this as a new column.

8. Load Data into MySQL 

Set Up Connections: Connected to MySQL  using sqlalchemy and loaded the cleaned data into each database.
Table Creation: Set up tables in  MySQL  using Python SQLAlchemy to automate table creation and data insertion.
Verification: Run initial SQL queries to confirm that the data has been loaded accurately.

9. SQL Analysis: Complex Queries and Business Problem Solving

Business Problem-Solving: Executed complex SQL queries to answer critical business questions, such as:
Revenue trends across branches and categories.
Identifying best-selling product categories.
Sales performance by time, city, and payment method.
Analyzing peak sales periods and customer buying patterns.
Profit margin analysis by branch and category.


## Results and Insights

This section includes analysis findings:
- **Sales Insights**:Sales are highest during the Afternoon shift, followed by Evening, and then Morning, suggesting most customers shop after mid-day.Each branch has a different peak day (e.g., Friday in one branch, Sunday in another), which helps in optimizing staffing and marketing campaigns.
  
- **Profitability**: Profitability varies by category. Some product categories yield significantly higher profit margins.Several branches showed a notable revenue drop from 2022 to 2023, helping identify underperforming locations.
  
- **Customer Behavior**: The most popular payment method varies by branch, with detailed transaction counts showing regional payment behavior.Customers prefer shopping in the afternoon, aligning with typical post-lunch hours, and showing when marketing efforts should peak.


---

## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart’s business case studies on sales and supply chain optimization.

---

