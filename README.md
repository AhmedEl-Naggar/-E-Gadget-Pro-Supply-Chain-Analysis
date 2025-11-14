Project Overview
This project analyzes the sales and supply chain operations of E-Gadget Pro, an online retailer of electronic goods. The goal is to consolidate multiple datasets, clean and process the data, uncover insights, and visualize key business metrics.
✅ Objectives

Combine sales data from multiple sources into a master dataset.
Perform data cleaning and calculate key metrics like revenue and profit.
Identify outliers and filter erroneous records.
Analyze top-performing categories, supplier performance, and monthly sales trends.
Create visualizations to present findings to management.


📂 Data Sources
The analysis uses four CSV files:

sales_part1.csv – Sales records for Jan–Jun.
sales_part2.csv – Sales records for Jul–Dec.
products.csv – Product details (name, category, cost, etc.).
suppliers.csv – Supplier details (name, location).


🛠️ Steps Performed
Step 1: Data Consolidation

Load all CSV files into Pandas DataFrames.
Merge sales data and enrich with product and supplier details.
Create a master DataFrame (master_df).

Step 2: Data Cleaning

Inspect data using .info() and .describe().
Add calculated columns:

revenue = quantity * sale_price
profit = (sale_price - cost_price) * quantity


Remove outliers where quantity > 50.

Step 3: Analysis

Top Performing Categories: Total revenue and profit by category.
Supplier Performance: Supplier generating the most revenue.
Monthly Sales Trend: Revenue trend across months.

Step 4: Visualization

Bar Chart: Total Revenue by Product Category.
Line Chart: Monthly Revenue Trend.


📦 Technologies Used

Python 3
Pandas for data manipulation
Matplotlib for visualization




📈 Output

Cleaned and consolidated dataset (master_df).
Visualizations:

Bar chart: Revenue by category.
Line chart: Monthly revenue trend.




🔍 Future Improvements

Automate data ingestion from APIs.
Add interactive dashboards using Plotly or Streamlit.
Implement predictive analytics for sales forecasting.
