📊 Superstore Sales & Performance Dashboard

🚀 OverviewThis project features an interactive and dynamic Power BI Dashboard built using the iconic Superstore dataset.
    The goal of this dashboard is to transform raw retail data into actionable business intelligence, helping stakeholders track key performance indicators (KPIs), analyze regional profitability, and uncover product-level insights to drive strategic decision-making.

🛠️ Tools & Technologies Used
    Data Visualization: Power BI DesktopData 
    Transformation & Modeling: Power Query, DAX (Data Analysis Expressions)
    Dataset Source: Superstore Dataset (CSV / Excel)
    Version Control: Git & GitHub

📈 Key Performance Indicators (KPIs)
    The dashboard tracks the following core metrics at a glance:
    Total Sales: Overall revenue generated.
    Total Profit: Net profit after all deductions.
    Total Quantity Sold: Total items purchased by customers.
    Profit Margin: Overall profitability percentage ($\text{Profit} / \text{Sales}$).
    Total Orders: Total number of transactions processed.

🔍 Dashboard Features & Insights
    Executive Summary: High-level overview of sales trends, profit margins, and monthly performance.
    Regional Analysis: Geographical breakdown of sales and profits across different states and regions using interactive maps.
    Category & Sub-Category Deep Dive: Identification of top-performing product categories (e.g., Technology, Office Supplies, Furniture) and loss-making sub-categories
    Customer Segmentation: Analysis of sales distribution across Consumer, Corporate, and Home Office segments.
    Interactive Filtering: Slicers for Date Ranges, Regions, Ship Modes, and Categories to dynamically slice the data.

🗂️ Data Modeling & DAX Measures
   Star Schema Architecture: The data model is structured around a central fact table (Sales) connected to dimension tables (Calendar, Customers, Products, Geography).
   Key DAX Measures Created:
   Total Sales = SUM(Sales[Sales])
   Total Profit = SUM(Sales[Profit])
   Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
   YTD Sales = CALCULATE([Total Sales], DATESYTD('Calendar'[Date]))



