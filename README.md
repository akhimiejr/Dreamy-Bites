# 1. Introduction
# Dreamy-Bites
Dreamy Bites is a premium cookie brand specializing in a variety of delectable treats, including chocolate chip, oatmeal raisin, and other gourmet cookies. The company  has earned a reputation for delivering top- notch products to retailers and customers  worldwide. 
# 1.1 Overview 
Dreamy Bites is a premium cookie brand offering a diverse range of gourmet products, including chocolate chip, oatmeal raisin, and other specialty cookies. The brand has built a strong reputation for delivering high-quality products to both retailers and customers across global markets. As the business continues to expand, gaining deeper insight into sales trends, customer behaviour, and product performance has become essential to support strategic and data-driven decision-making.
However, Dreamy Bites currently faces challenges in consolidating its business data, which is dispersed across multiple sources. Product information and updated pricing are stored in a PDF document, customer details are maintained in a CSV file, and order transactions—including quantities and payment information—are recorded in a Google Sheet. This fragmented data structure limits efficient reporting, slows analysis, and makes it difficult to identify performance trends and growth opportunities
# 1.2 Aim of the Project
To integrate these diverse data sources into a
unified Power BI report, enabling Dreamy
Bites to:
• Analyze sales performance across products
and regions.
• Gain insights into customer demographics
and purchasing patterns.
• Track and manage order trends to optimize
inventory and delivery processes.
• Generate actionable reports to support
strategic planning and growth initiatives.
# 1.3 Data Description
 We have been given 3 tables from different sources;
• Orders table – A fact table that contains all the business transactions for 16 months(Sept 2019 – Dec 2020)
• Customers table – A dimension table that contains all thepersonal information of the retailers
• Cookies table – A dimension table that contains the production and selling cost of each product
##### Order Table
• Customer ID: A unique identifier that
links each order to a specific customer
• Order ID: A unique identifier assigned
to every order placed
• Product: The name or type of cookie
purchased in the order
• Units Sold: The quantity of a particular
cookie product sold in the specific
order.
• Date: The date when the order was
placed.
##### Product Table
• Product: The type or name of the
cookie (e.g., Chocolate Chip, Fortune
Cookie).
• Selling Cost Per Cookie: The retail
price at which a single cookie is sold to
customers
• Production Cost Per Cookie: The cost
incurred by the company to produce a
single cookie, including ingredients
and labor.
##### Customer Table
• Customer ID: A unique identifier for each customer
• Name: The full name of the customer who placed the order.
• Phone: The contact number provided by the customer
• Address: The street address where the customer resides or where the order may be
delivered.
• City: The city where the customer is located.
• State: The state of residence for the customer.
• Zip: The postal or ZIP code for the customer's address
• Country: The country where the customer resides.
• Notes: Any additional information or comments about the customer, such as
preferences or special requests.
# 2. Analysis
## 2.1 Problem Statement
Dreamy Bites faces a challenge in consolidating its data,
which is currently scattered across multiple sources:
• A PDF file containing product descriptions and their
updated sales prices.
• A CSV file storing customer information
• A Google Sheet that tracks orders, including
quantities and payment details.
This fragmentation hinders efficient reporting, decision-
making, and the identification of growth opportunities.
## 2.2 Data Modelling 
The data model shows a classic star schema, with the Order_Fact table at the centre capturing transactional data such as Order ID, Date, Expenses and Product. This fact table is linked via one-to-many relationships to the Customers_Dim table (containing customer attributes such as name, location and contact details) and the Product_Dim table (holding product types and unit-level production and selling costs). A dedicated Measures table is used to store calculated metrics, improving model clarity, reusability, and performance. This structure enables consistent filtering across visuals and underpins the slicers used in both dashboards.

<img width="1495" height="630" alt="Screenshot 2026-01-08 143222" src="https://github.com/user-attachments/assets/00ba973d-18c6-4384-9af6-b2ce9d7caa80" />

# 3. Dashboard Reporting
## 3.1 Product Performance Analysis
The Product Analysis dashboard shifts focus to product performance while maintaining consistency in design and metrics. KPI cards summarise Total Profit (£3M), Total Orders (700), Total Expenses (£1.97M) and Number of Products (6), alongside order contribution metrics. A combined area and line chart tracks monthly total profit and quantity sold, revealing seasonal patterns and peak performance periods. Product-level bar charts compare expenses versus profit by product, highlighting cost efficiency and margin differences between cookie types. Additional visuals show quantity sold by product and rank products by total volume, making it easy to identify best-selling and underperforming items. A Name slicer allows users to filter the dashboard by customer, ensuring seamless cross-analysis between customer and product perspectives.

<img width="1159" height="675" alt="Screenshot 2026-01-08 143517" src="https://github.com/user-attachments/assets/52387994-770f-4a32-ae08-4f89bacc2594" />

## 3.2 Customer performance Analysis
The Customer Analysis dashboard focuses on customer-level performance. KPI cards at the top summarise headline metrics, including Total Profit (£3M), Total Orders (700), Total Customers (5) and Total Expenses (£1.97M). Gauge visuals provide immediate context by comparing Customer Profit against a target and showing Total Quantity Sold (1,125,824 units) against an upper benchmark. A geographical map visual displays customer profit by state, highlighting regional concentration and performance differences across the United States. Below, bar charts break down total expenses versus profit by customer, clearly illustrating margin performance for each customer, while additional visuals show quantity sold by customer name and number of orders per customer, allowing easy identification of high-volume and high-frequency buyers. A Product slicer enables users to dynamically filter all visuals to analyse customer behaviour for specific products.

<img width="1149" height="676" alt="Screenshot 2026-01-08 143448" src="https://github.com/user-attachments/assets/1e82bfac-afea-4072-ac85-dc9e82183a9b" />
