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
