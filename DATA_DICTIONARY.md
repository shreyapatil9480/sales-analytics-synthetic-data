# Data Dictionary

This file describes each column in the `synthetic_sales_data.csv` dataset.

| Column | Description |
| --- | --- |
| **Date** | Date of transaction (YYYY-MM-DD) |
| **Product_ID** | Unique identifier for each product |
| **Product_Category** | Category of product (Electronics, Clothing, Home & Kitchen, Sports, Beauty) |
| **Customer_Age** | Age of the customer in years |
| **Customer_Gender** | Gender of the customer (Male/Female) |
| **Region** | Geographic region where the sale occurred (North, South, East, West, Central) |
| **Season** | Season of the transaction (Winter, Spring, Summer, Autumn) |
| **Sales_Quantity** | Number of units sold |
| **Unit_Price** | Price per unit (USD) |
| **Discount** | Discount applied to the sale (0–0.30) |
| **Total_Sales** | Total revenue for the sale after discount (Sales_Quantity × Unit_Price × (1 – Discount)) |
| **Advertising_Spend** | Advertising or marketing spend associated with the sale |
| **Cost_per_unit** | Cost to produce or procure each unit |
| **Profit** | Profit from the sale (Total_Sales – Sales_Quantity × Cost_per_unit) |
| **Profit_Margin** | Profit divided by Total_Sales |
