
# SWYNEX – Final Data Analytics Project
## Blinkit Product Sales and Performance Analysis

## 1. Project Overview

This project was completed as part of my internship with SWYNEX Technologies.

The objective of this project is to perform end-to-end data analytics on a Blinkit product dataset. The project includes data cleaning, exploratory data analysis (EDA), data visualization, an interactive Tableau dashboard, and business insights.

The analysis helps explore product sales, pricing, customer ratings, discounts, stock levels, demand, and delivery performance.

## 2. Problem Statement

Retail businesses need to understand product sales, pricing, inventory demand, and delivery performance to make better business decisions.

Unclean data and limited visibility into product performance can make it difficult to identify top-selling categories, high-performing cities, and potential operational issues.

This project uses Python, Pandas, and Tableau to prepare and analyze the Blinkit dataset and present the findings through an interactive dashboard.

## 3. Project Objectives

- Clean and prepare the raw dataset.
- Identify and handle missing values.
- Check duplicate records and data types.
- Perform exploratory data analysis using Python.
- Calculate important statistical measures.
- Identify trends, patterns, and unusual values.
- Build an interactive Tableau dashboard.
- Present useful business insights from the analysis.

## 4. Dataset Information

The project uses the Blinkit product dataset selected for the data cleaning task.

- **Number of records:** 13,000
- **Number of columns:** 25
- **File format:** CSV
- **Dataset used for analysis:** Blinkit_Cleaned_Data.csv

The dataset contains information about products, categories, brands, prices, discounts, ratings, sales quantities, delivery times, stock, demand, and delivery status.

Important columns include:

- `product_name`
- `category`
- `brand`
- `price`
- `discount_pct`
- `final_price`
- `rating`
- `sold_quantity`
- `delivery_time_min`
- `city`
- `stock`
- `profit_margin_pct`
- `demand_index`
- `delivery_status`

## 5. Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Tableau
- Git
- GitHub

## 6. Data Cleaning and Preparation

Data cleaning was performed using Python and Pandas.

The following steps were completed:

1. Loaded the dataset into a Pandas DataFrame.
2. Inspected the dataset structure, column names, and data types.
3. Identified missing values.
4. Filled missing values in `offer_type` with `No Offer`.
5. Checked for duplicate records.
6. Converted `date_added` and `expiry_date` to datetime format.
7. Checked categorical values for consistency.
8. Removed unnecessary leading and trailing spaces from text columns.
9. Validated numerical fields, including price, discount, and rating.
10. Checked the relationship between price, discount percentage, and final price.
11. Validated date consistency.
12. Performed final data quality checks and exported the cleaned CSV.

### Data Cleaning Results

- Original dataset size: 13,000 rows and 25 columns.
- Missing values in `offer_type`: 6,544.
- Missing values after cleaning: 0.
- Exact duplicate records found: 0.
- Records with expiry dates earlier than their added dates: 0.
- Date columns converted to datetime format.

The stored `final_price` values were checked against the calculated discounted prices. Differences were identified in 246 records and were retained for review rather than automatically overwritten.

## 7. Exploratory Data Analysis (EDA)

Exploratory data analysis was performed using Pandas, NumPy, and Matplotlib.

The analysis included:

- Sales by product category.
- Sales by city.
- Top-selling products.
- Product rating distribution.
- Discount percentage versus sold quantity.
- Delivery time distribution.
- Stock levels versus demand.
- Summary statistics for price, ratings, sales, and profit margin.

### Key Statistical Results

| Metric | Result |
|---|---:|
| Total sold quantity | 2,111,201 |
| Average price | 267.30 |
| Average final price | 240.74 |
| Average product rating | 4.20 |
| Average delivery time | 27.56 minutes |
| Average profit margin | 22.65% |

These figures describe the dataset before interactive dashboard filters are applied.

## 8. Key Business Insights

### 1. Sales by Category

Bakery recorded the highest total sold quantity at 273,416 units, followed by Grocery at 273,006 units.

**Business implication:** Retailers can compare category performance when planning inventory and promotions.

### 2. Sales by City

Mumbai recorded 219,930 units sold, followed by Bengaluru at 217,651 units.

**Business implication:** City-level sales comparisons can help businesses investigate regional demand and plan stock allocation.

### 3. Top-Selling Product

Lizol Fresh Household 484 recorded 967 units sold, making it the top-selling product identified in the analysis.

**Business implication:** High-selling products can be monitored carefully to reduce the risk of stock shortages.

### 4. Product Ratings

The average product rating was 4.20.

**Business implication:** Businesses can examine ratings alongside sales to understand product performance and identify products that may need further investigation.

### 5. Delivery Performance

The average delivery time was 27.56 minutes, with observed delivery times ranging from 10 to 56 minutes.

**Business implication:** Delivery times can be monitored to identify slower deliveries and opportunities for operational improvement.

### 6. Profit Margin

The average profit margin percentage was 22.65%.

**Business implication:** Comparing profit margin with sales volume can help businesses evaluate product performance and pricing decisions.

### 7. Product Demand

Several products recorded a demand index of 100, the highest observed value in the dataset.

**Business implication:** Products with high demand indicators can be monitored when planning stock and replenishment.

## 9. Interactive Tableau Dashboard

The Blinkit Product Dashboard was created using Tableau to present the analysis in an interactive format.

### Dashboard KPIs

- Total Sold Quantity
- Average Price
- Average Final Price
- Average Rating
- Average Delivery Time

### Dashboard Visualizations

- Sales by Category
- Sales and Profit by City
- Top 10 Products by Sales
- Discount vs Sales
- Stock vs Demand
- Delivery Status Distribution

### Interactive Filters

- City
- Category
- Brand
- Offer Type
- Is Organic
- Delivery Status

The filters allow users to explore different categories, cities, brands, and delivery conditions.

## 10. Dashboard Screenshot

## Blinkit Product Dashboard 

![alt text](<Updated Blinkit_Product_Dashboard.png>)

The dashboard presents key performance indicators and charts to help users explore product sales, pricing, demand, and delivery performance.

## 11. Project Workflow

1. Select the dataset.
2. Inspect and clean the data using Python and Pandas.
3. Validate data quality and export the cleaned CSV.
4. Perform exploratory data analysis.
5. Calculate statistics and create charts.
6. Identify important business insights.
7. Build the interactive Tableau dashboard.
8. Document the project and upload files to GitHub.

## 12. Key Learnings

Through this project, I gained practical experience in:

- Data cleaning and preparation using Pandas.
- Exploratory data analysis.
- Statistical analysis and data validation.
- Creating charts and visualizations.
- Designing KPI cards and interactive dashboards in Tableau.
- Identifying and communicating business insights.
- Organizing and documenting projects using Git and GitHub.

## 13. Conclusion

This project demonstrates an end-to-end data analytics workflow, from raw dataset preparation to exploratory analysis and interactive dashboard development.

The analysis highlights differences in product category sales, city performance, product demand, pricing, and delivery times. These findings can help guide further investigation and support data-informed retail decisions.

## 14. Repository Structure

```text
SWYNEX-Final-Data-Analytics-Project/
├── data/
│   └── Blinkit_Cleaned_Data.csv
├── notebooks/
│   ├── data_cleaning.ipynb
│   └── blinkit_eda.ipynb
├── Dashboard/
│   └── Blinkit Product Dashboard.twbx
├── Screenshot/
│   └── Blinkit_Product_Dashboard.png
├── README.md
└── requirements.txt
```

## Author

Darshan RN

## Internship

SWYNEX Technologies
