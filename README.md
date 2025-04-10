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

# Methodology
Data Cleaning & Preprocessing:

Handled missing values using appropriate imputation techniques.

Derived new metrics such as delivery delay and customer age (calculated as the difference between creationDate and dateOfBirth).

Grouped raw size data into standardized categories to facilitate analysis.

Data Visualization:

Developed interactive dashboards using Power BI to visualize:

Delivery performance vs. return rates.

Size & fit issues across different product categories.

Return patterns by price, manufacturer, customer demographics, and regional differences.

Analysis & Insight Extraction:

Analyzed correlations between late deliveries, size mismatches, price fluctuations, and return rates.

Evaluated the impact of customer demographics and regional differences on return behavior.

Synthesized findings into actionable recommendations.

# Key Findings
Late Delivery:
Orders delivered later than 10 days are significantly more likely to be returned, suggesting that delays lead to customer dissatisfaction and increased costs.

Size & Fit Issues:
Items in extreme size categories (sizes less than 34, as well as L and XXXL) show notably higher return rates, highlighting potential sizing inaccuracies or fit issues.

Price & Manufacturer Fluctuations:
Higher-priced items tend to have higher return rates. Additionally, return rates vary widely by manufacturer, indicating significant differences in product quality and design consistency.

Customer Demographics & Regional Differences:
Middle-aged customers (ages 30 to 60) display more stable and lower return rates compared to younger or older customers. Specific regions like Saxony and Thuringia have higher return rates, and female customers in certain regions (e.g., Saxony-Anhalt) tend to return products more frequently.

# Technologies Used
Data Cleaning & Analysis: Python (Pandas, NumPy)

Data Visualization: Power BI

![Screenshot (139)](https://github.com/user-attachments/assets/1e8f3543-0a9d-4f8a-9a7c-716df343248f)
