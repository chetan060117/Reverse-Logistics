# Reverse-Logistics

# Optimizing Reverse Logistics through Data Visualization
# Project Overview

ABC Logistics, a major e-commerce fulfillment and shipping company, was facing increasing product return rates. This project analyzed a comprehensive dataset to identify the key drivers behind returns and provided actionable recommendations to optimize reverse logistics. By leveraging data cleaning, grouping, and interactive visualizations, the project revealed critical insights about delivery performance, size & fit issues, price and manufacturer fluctuations, and customer demographics & regional differences.

# Dataset Description

Size: 481,092 rows and 14 columns

Key Attributes:

Order Details: orderItemID, orderDate, deliveryDate, price, manufacturerID

Customer Information: customerID, salutation, dateOfBirth, creationDate, state

Product Attributes: itemID, size, color

Return Data: returnShipment, delay

Data Issues & Cleaning:

Missing Values:

deliveryDate: 39,419 null values

color: 143 null values

dateOfBirth: 48,889 null values

Imputation:

Mode imputation was used for the color column.

For date columns, imputed missing dateOfBirth as creationDate - 47 years and deliveryDate as orderDate + 10 days.

Size Grouping:

The size column was grouped into categories (others, XS, S, M, L, XL, XXL, XXXL, Outlier, Unsized) to create a new field SizeCategory.

