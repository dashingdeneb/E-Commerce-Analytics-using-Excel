# E-Commerce-Analytics-using-Excel
E-Commerce Analytics using Excel

**Problem Statement**
We are tasked with analyzing StellarMart's business data to provide actionable insights for strategic growth. StellarMart is a mid-sized retail chain specializing in Electronics, Clothing, Home Appliances, Books, and Groceries. Faced with growing competition and shifting customer preferences, the company aims to leverage data-driven insights to optimize operations and boost profitability. As a data analytics consultant, your role is to transform two years of raw sales, customer, and product data into meaningful insights.

**Business Problem**
StellarMart has been experiencing challenges in several areas:
- **Sales Decline in Certain Product Categories:** While some categories perform exceptionally well, others show stagnation or decline. Management wants to know which categories and products are thriving and which require strategic intervention.
- **Seasonal Trends:** StellarMart suspects sales trends fluctuate significantly by season or time of year but lacks clear visibility into these patterns.
- **Regional Performance:** Different regions contribute unequally to overall revenue, and StellarMart wants to prioritize investment in high-performing areas while addressing underperformance

**Role**
Analyze StellarMart’s data and address the following objectives:

- Identify sales trends over time, including monthly and seasonal fluctuations.
- Compare sales performance across product categories and pinpoint underperforming ones.
- Analyze sales contributions category wise from each region
- Create dynamic visualizations to showcase key insights (e.g., sales trends, customer segmentation, and regional performance).


**1. Data Cleaning**

    Remove Duplicate Rows
        Select the dataset.
        Use the "Remove Duplicates" option under the Data tab, ensuring all columns are checked.
    Handle Missing Values
        Identify missing values in key columns like "Category," "Region," and "Product Name."
        Replace missing values with defaults or remove rows with critical missing data.
    Correct Inconsistent Text Formatting
        Standardize text using formulas (e.g., REPLACE function).
        Fix inconsistencies like lowercase or typos.
    Fix Typos in Product Names
        Use string functions like REPLACE/TRIM to clean suffixes or fix variations.
    Ensure Data Consistency
        Verify product-to-category assignments using VLOOKUP or manual corrections.

**2. Data Preprocessing**

    Add Time-Based Columns
        Extract "Month-Year" using: =TEXT(Date, "mmm yyyy").
        Add "Quarter-Year" using: ="Q"&ROUNDUP(MONTH(Date)/3,0)&" "&TEXT(Date,"YY").

**3. Sales Analysis**

    Analyze Sales by Category and Region
        Use a PivotTable:
            Rows: Category, Region.
            Values: Total Sales (Sum), Sale Price (Average), Quantity Sold (Sum).
    Compare Sales Performance
        Highlight sales trends and prioritize high- or low-performing areas.
        Sort PivotTables by "Total Sales" for actionable insights.

**4. Data Visualization**

    Create Charts
        Stacked bar/column chart: Sales by Category and Region.
        Pie chart: Customer Segmentation.
        Horizontal bar chart: Top Products.
