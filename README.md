Ecommerces Sales Projects.




Ecommerce Sales Dashboard designed for deep and insightful business analysis

This dashboard was created using real-world ecommerce data and showcases.

Key Components of the Dashboard
📊 1. Top KPI Cards
At the top, we have Key Performance Indicators (KPIs):

Num Customers: 29K
Num Transactions: 54K
Avg Sales per transaction: ₹3,000
Total Sales: ₹160.74M
Avg Discount: ₹136.92
These metrics give you an executive summary at a glance.

🧓👩‍🦰 2. Total Sales by Age Group
A bar chart showing how different age groups contribute to total sales:

Highest spenders: 25–45 years
Lower sales from under 18 and 60+
📅 3. Sales Over Time
The line chart reveals trends in total sales by:

Year
Quarter
Month
You can observe sales growth, seasonality, and spikes across years (2019–2024).

💳 4. Total Sales by Purchase Method
Insights into customer preferences:

Most used: Credit Card, Debit Card
Least used: Google Pay, Paytm, and Cash on Delivery
👩‍🦱🧔 5. Sales by Gender
A pie chart highlighting the gender split:

Slightly more sales by Females (54%)
🏷️ 6. Discount Analysis
Understand how offering discounts influences total sales:

Avg Sales for users who availed discounts is ₹3,000
🗺️ 7. Sales by Location
A map visualization shows geographic distribution across India and neighboring countries.

📦 8. Sales by Product Category
A treemap to break down top-selling categories:

Electronics and Clothing are leading
Books, Toys, and Sports follow
🎯 Filters / Slicers (on the right):
Allow dynamic filtering by:

Age Group
Discount Availed
Gender
Location
Purchase Date (with a date slider)
----------------------------------------------------------
DAX Page 
📊 1. Top KPI Cards 

Num Customers: 29K
Num Transactions: 54K
Avg Sales per transaction: ₹3,000
Total Sales: ₹160.74M
YoY Growth = -83.10%

1. Cy sale and py sales Month comapresion in line chart.

CY Sales = CALCULATE([Total Sales],
YEAR( 'Ecommerce Sales'[Purchase Date] ) = 2024),

PY Sales = CALCULATE([Total Sales], 
SAMEPERIODLASTYEAR('Ecommerce Sales'[Purchase Date].[Date]))

YOY Growth % = DIVIDE([CY Sales] - [PY Sales],[PY Sales],0)

2. category % by Product category copmare in stack bar chart.

Category Sales % = DIVIDE([Total Sales], CALCULATE( [Total Sales], 
ALL('Ecommerce Sales'[Product Category])),0) 

3. Sales per customer % by age group 

Sales Per Customer % = DIVIDE( [Total Sales], [No Of Customers],0)

----------------------------------------------------------------------------------------------------------------------------------------------



