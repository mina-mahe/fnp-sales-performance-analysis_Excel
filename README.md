# Ferns and Petals (FNP) Sales Analysis Dashboard

## Project Overview
This project involves a comprehensive sales analysis for Ferns and Petals (FNP), specializing in gift delivery for various occasions. The goal was to transform raw transactional data into actionable business insights regarding sales trends, customer behavior, and operational efficiency.

## Technical Toolstack
* **Power Query**: Data cleaning, ETL, and merging of disparate datasets (Customers, Orders, Products).
* **Power Pivot (DAX)**: Data modeling and creation of calculated columns for Revenue and Order Weekday.
* **Excel Dashboards**: Interactive visualization using Slicers, Pivot Charts, and Timelines.

## Data Transformation (ETL)
Using Power Query, I performed the following steps to ensure data integrity:
* **Column Profiling**: Verified 100% data quality with no errors or empty values in core fields.
* **Feature Engineering**: 
    * Calculated `Diff_Order_Delivery` to measure logistical lead times.
    * Extracted `Order_Hour` and `Month Name` for temporal trend analysis.
    * Merged Product and Order tables to pull `Price (INR)` into the transaction log.
* **Data Modeling**: Established a **Star Schema** in Power Pivot, linking fact tables (Orders) to dimension tables (Customers, Products) via `Customer_ID` and `Product_ID`.
<img width="1473" height="703" alt="Screenshot (176)" src="https://github.com/user-attachments/assets/61a94386-dcc4-4299-bc65-ef3510a10d87" />


## Key Business Insights & Interpretations

### 1. Financial Performance
* **Total Revenue**: ₹35,20,984.00 across 1,000 total orders.
* **Average Customer Spending**: ₹3,520.98.
* **Top Category**: **Colors (29%)** and **Sweets/Soft Toys (21% each)** drive the bulk of the revenue.

### 2. Operational Efficiency (Delivery Time)
* **Average Delivery Time**: 5.53 days.
* **Correlation Analysis**: The correlation between `Order Quantity` and `Delivery Time` is **0.0035**.
    * **Interpretation**: There is almost **zero correlation**. This suggests that larger order quantities do not significantly delay delivery times, indicating a scalable logistics process.

### 3. Temporal & Occasion Trends
* **Peak Sales Months**: February (Valentine's) and August (Raksha Bandhan) showed the highest spikes in monthly performance.
* **Hourly Activity**: Order volume peaks around **7 PM (19:00)** and **7 AM (07:00)**, suggesting customers prefer shopping at the start or end of their day.
* **Top Occasions**: **Anniversary** and **Raksha Bandhan** are the highest revenue-generating occasions.

### 4. Customer Demographics
* **Gender Distribution**: Revenue is almost perfectly balanced between genders (Male: ₹17.9L vs. Female: ₹17.3L), suggesting a neutral marketing appeal.
* **Geographic Focus**: Imphal and Dhanbad are among the top cities by order volume, indicating strong market penetration in these regions.
  
## Final Dashboard
<img width="1821" height="874" alt="FNP_Sales_Analysis_Dashboard" src="https://github.com/user-attachments/assets/dc4ac11c-48cb-4c6f-9922-3a1716adb9b6" />

*Developed as part of a Data Analytics Portfolio.*
