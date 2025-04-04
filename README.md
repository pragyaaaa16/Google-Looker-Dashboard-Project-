Project Title:
Advanced Sales Analytics with Google Looker Studio Click on the below link to view the dashboard:
https://lookerstudio.google.com/s/i9OZNghMYJY

Project Description:
This project involves analyzing sales data from a retail company to derive actionable insights and create impactful visualizations using SQL, Python, and Google Looker Studio. The dataset comprises multiple tables (customer_detail, order_detail, sku_detail, and payment_detail) representing customers, orders, products, and payments. The objectives of this project include:
1. Deriving Key Insights:
Identifying top-performing products, analyzing category-wise trends, improving decision-making, compare sales of 2021 and 2022, find customers across different segments and finding avergae sales for each product to help restack the correct products.

2. Visualizing Data:
Creating interactive dashboards in Google Looker Studio for better understanding and presentation of data.

3. Customer Behavior Analysis:
Highlighting customer payment patterns to support targeted marketing campaigns.

Pre-requisites:
Before starting this project, you should have the following knowledge and tools in place:

1. Basic SQL Knowledge:
o Understanding of SQL queries such as SELECT, JOIN, GROUP BY, and filtering data using WHERE and HAVING. o Familiarity with creating and managing relational databases and tables.

2. Basic Python Skills:
o Knowledge of Python and libraries such as Pandas for data manipulation and Matplotlib/Seaborn for basic visualizations. o Experience in handling data frames and performing data cleaning and transformation tasks.

3. Google Looker Studio:
o Familiarity with Google Looker Studio (formerly Google Data Studio) for creating interactive dashboards and visualizations. o Knowledge of connecting data sources and building dynamic reports.

4. Data Analysis Concepts:
o Understanding basic data analysis techniques, such as identifying trends, comparing time periods, and aggregating data to derive insights. o Familiarity with metrics like growth percentages, total sales, and performance benchmarks.

5. Tools & Technologies:
o SQL Database: A SQL-based database to store and query the data. o Python: IDE or environment (e.g., Jupyter Notebook, Google Colab) for running Python scripts. o Google Looker Studio: A Google account and access to Looker Studio for creating and sharing dashboards.

Key Steps and Analysis
Data Preparation:
1. Database Setup:
o Designed the sales database with normalized tables to ensure scalability and efficiency. o Key tables include: ▪ customer_detail: Customer information. ▪ order_detail: Order transactions. ▪ sku_detail: Product details like categories and pricing. ▪ payment_detail: Payment methods and statuses.

2. Data Transformation with Python:
o Extracted data using SQL queries and processed it with Python for cleaning and enrichment. o Calculated features like qty_growth and delta_2022_2021 to measure performance trends.

Analysis and Visualization:
1. Top Product Analysis (2022):
o Used SQL and Python to identify Top 5 products in the "Mobiles & Tablets" category by sales quantity. o Visualized results with bar charts using Python libraries like Matplotlib and Seaborn.

2. Category Trend Analysis (2021 vs. 2022):
o Compared category-wise sales growth or decline between 2021 and 2022. o Focused on the "Others" category to identify the Top 20 products with the largest sales decline. o Generated horizontal bar charts for side-by-side comparison.

3. Customer Payment Behavior:
o Identified customers who completed the checkout process (is_gross = 1) but had pending payments. o Created customer segments for targeted follow-ups.

4. Google Looker Studio Dashboards:
o Designed and published interactive dashboards to present key findings. o Integrated the data with Looker Studio to showcase: ▪ Year-on-year sales performance by category. ▪ Top-performing products and declining trends. ▪ Customer payment patterns and overdue payments. o These dashboards allow dynamic filtering, exploration of data, and easy sharing with stakeholders for better decision-making.

Tasks:
Task 1: Sales Decline in "Others" Category (2021 vs. 2022)
Steps: 
1. Filtered sales data for "Others" (2021 vs. 2022).  
2. Calculated sales difference and % change.  
3. Classified trends as "DOWN," "UP," or "FAIR".  
4. Visualized top 20 declining products in a horizontal bar chart.  

Key Features:  
- Date filtering (`EXTRACT(YEAR FROM order_date)`).  
- Calculated fields for YoY comparison.
  
Task 2: Customer Profitability Segmentation
Steps:
1. Calculated net profit per customer:  
   ```sql
   SUM(after_discount - cogs)
   ```  
2. Segmented customers:  
   - Low: < $100  
   - Medium: $100–$500  
   - High: > $500  
3. Created a pie chart for segment distribution.  

Key Features: 
- CASE statements for segmentation.  
- Pie chart styling (colors, % labels).
  
Task 3: Average Quantity Sold per Product Category
Steps:
1. Calculated average quantity sold per category:  
   ```sql
   AVG(qty_ordered)
   ```  
2. Sorted categories descending by average sales.  
3. Created a bar chart to highlight top/low performers.  

Key Features: 
- Dimension: `category`  
- Metric: `AVG(qty_ordered)`  
- Sorting and slanted x-axis labels for readability.  

Insight:
- Identified top-selling categories needing stock prioritization.  
- Flagged low-performing categories for review.  


Tools and Technologies Used:
• SQL:
o Database creation, querying, and aggregation. o Extracted data using JOIN, GROUP BY, and advanced filtering.

• Python:
o Data processing with Pandas for cleaning and transformation. o Visualization using Matplotlib and Seaborn for detailed insights.

• Google Looker Studio:
o Created interactive dashboards with real-time filters and drill-down capabilities. o Integrated SQL-based data for visualization and easy sharing with stakeholders.

Key Deliverables:
1. Actionable Insights:
o Identified top products and categories driving revenue. o Highlighted trends and anomalies for inventory optimization and targeted promotions.

2. Interactive Dashboards:
o Real-time data exploration via Google Looker Studio dashboards. o Easy-to-navigate visualizations for stakeholders.

3. Customer Targeting Recommendations:
o Identified customers for payment follow-ups, optimizing cash flow and sales conversions.

Skills and Competencies  
- Looker Studio: Advanced calculated fields, interactive dashboards.  
- Data Storytelling: Translating trends into business actions.  
- Collaboration: Aligning with Warehouse, Marketing, and Product teams.

Feedback and Evidence
- Product Team: Used average quantity data to adjust procurement.  
- Screenshots: Shared dashboards showing YoY trends and category performance.

Challenges and Solutions
Challenge	Solution
Data Discrepancies in “Others” category	Validated SKUs with the Warehouse team
Slow dashboard loading	Reduced granularity by pre-aggregating data
	
Outcomes and Impact 
- 15% reduction in excess inventory for "Others" category.  
- 20% increase in marketing engagement from High-profit customers.  
- Faster decision-making with real-time dashboards.
  
Conclusion
This internship honed my ability to turn raw data into strategic insights, impacting inventory, marketing, and product strategies. I’m now proficient in **Looker Studio, Python analytics, and cross-functional collaboration.  

Impact:
The project empowers stakeholders with actionable insights and interactive visualizations, supporting strategic decisions in marketing, sales, and customer management. Google Looker Studio dashboards make the data easily accessible and interpretable, fostering data-driven strategies for better business outcomes.
