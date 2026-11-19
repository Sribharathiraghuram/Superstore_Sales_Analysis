# Superstore Sales Analysis
### Exploratory Data Analysis Using Python

**Project Name:** Superstore Sales Analysis  
**Author:** Sri Bharathi  
**Project Type:** Data Analytics – Exploratory Data Analysis (EDA)  
**Primary File:** `Superstore_Sales_Analysis.ipynb`  
**Dataset File:** `superstore_sales.csv.xlsx`

---

## 1. Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on a Superstore sales dataset using Python. The objective is to analyze sales, profit, customer purchasing behaviour, product category performance, regional performance, and discount impact to identify meaningful business insights.

The analysis involves data cleaning, data transformation, statistical exploration, and data visualization to understand business performance and support data-driven decision-making.

## 2. Business Objectives

The main objectives of this project are:

- Analyze overall sales and profit performance.
- Identify monthly and yearly sales trends.
- Understand sales and profit performance across product categories.
- Compare business performance across different regions.
- Analyze customer segment purchasing behaviour.
- Evaluate the impact of discounts on profitability.
- Identify relationships between numerical variables.
- Detect potential outliers in sales and profit data.
- Provide actionable business recommendations based on the analysis.

## 3. Tools and Technologies

The following tools and technologies were used:

| Tool / Technology | Purpose |
|---|---|
| Python | Data analysis and programming |
| Pandas | Data manipulation and cleaning |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Jupyter Notebook | Development and analysis environment |

## 4. Dataset Description

The project uses a Superstore sales dataset containing information about customer orders, products, sales, discounts, profits, and geographical regions.

**Original Dataset Dimensions:**
- Rows: 10,800
- Columns: 21

**Important Dataset Features:**
- Order ID
- Order Date
- Ship Date
- Ship Mode
- Customer ID
- Customer Name
- Segment
- Country
- City
- State
- Region
- Product ID
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Discount
- Profit

The dataset was used to explore different aspects of business performance and customer purchasing patterns.

## 5. Data Cleaning and Preparation

Data cleaning and preparation were performed to improve data quality and make the dataset suitable for analysis.

The following steps were completed:

- Imported the required Python libraries.
- Loaded the Superstore dataset using Pandas.
- Inspected the dataset structure using `head()`, `info()`, and `describe()`.
- Checked for missing values.
- Identified and removed records with missing Order Date values.
- Checked for duplicate records.
- Converted the Order Date column into datetime format.
- Extracted Year, Month, Month Name, and Year-Month from the Order Date column.
- Retained the remaining missing Postal Code values because they were not required for the main analysis.

**Dataset after cleaning:**
- Original records: 10,800
- Records removed due to missing Order Date: 806
- Final records: 9,994
- Remaining missing Postal Code values: 11
- Exact duplicate records: 0

## 6. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand business performance and identify important patterns in the dataset.

### 6.1 Overall Business Performance

Analyzed the overall sales, profit, profit margin, and order count to understand the business's overall performance.

### 6.2 Monthly Sales Analysis

Analyzed monthly sales trends to identify high-performing and low-performing months and understand sales seasonality.

### 6.3 Category-wise Sales and Profit Analysis

Compared sales and profit across different product categories to identify the categories contributing most to business performance.

### 6.4 Regional Sales and Profit Analysis

Analyzed sales and profitability across different geographical regions to understand regional business performance.

### 6.5 Customer Segment Analysis

Compared sales, profit, and quantity across customer segments to understand customer purchasing behaviour.

### 6.6 Discount Sensitivity Analysis

Examined the relationship between discount levels and profitability to understand how discounts affect business performance.

### 6.7 Correlation Analysis

Used correlation analysis to examine relationships between numerical variables such as Sales, Profit, Quantity, and Discount.

### 6.8 Outlier Analysis

Used statistical techniques, including the Interquartile Range (IQR) method, to identify potential outliers in Sales and Profit data.

## 7. Dashboard and Data Visualization

A business dashboard was created using Matplotlib to present important business performance indicators and trends in a clear and understandable format.

The dashboard includes:

- Monthly Sales Trend
- Category-wise Sales
- Region-wise Profit
- Customer Segment Sales
- Key Performance Indicators (KPIs)

Additional visualizations were created using Seaborn to explore sales patterns, discount impact, correlations, and potential outliers.

## 8. Key Business Insights

The analysis produced the following findings:

### Overall Performance
- Total Sales: **$2,297,200.86**
- Total Profit: **$286,397.02**
- Overall Profit Margin: **12.47%**
- Total Orders: **5,009**

### Monthly Sales Trends
- November recorded the highest combined monthly sales.
- February recorded the lowest combined monthly sales.
- November 2018 was the highest-performing month, with sales of approximately $89,306.24.
- February 2015 recorded the lowest monthly sales, at approximately $12,743.11.

### Category Performance
- Technology generated the highest sales and profit among the product categories.
- Furniture had a relatively low profit margin of approximately 2.49%, indicating an opportunity to improve profitability.

### Regional Performance
- The West region recorded the highest sales and profit.
- The Central region recorded the lowest profit among the regions.

### Customer Segment Performance
- The Consumer segment contributed the highest sales, profit, and quantity among the customer segments.

### Discount Impact
- Orders with no discount generated the highest total profit among the discount groups.
- Higher discount levels were associated with weaker profitability.
- Records with discounts of 30% or more had a combined negative profit of approximately $135,376.06.

### Correlation and Outliers
- Sales and Profit showed a positive correlation.
- Discount and Profit showed a negative correlation.
- Potential outliers were identified in both Sales and Profit data and retained for analysis.

## 9. Business Recommendations

Based on the findings, the following recommendations can help improve business performance:

1. **Improve Furniture Profitability:** Review Furniture pricing, product costs, and operational expenses to improve its low profit margin.

2. **Optimize Discount Strategies:** Evaluate high-discount transactions and introduce more controlled discount policies to reduce profit losses.

3. **Focus on High-Performing Categories:** Continue supporting the Technology category while identifying opportunities to improve the performance of other categories.

4. **Strengthen Regional Strategies:** Study successful business practices in the West region and identify improvement opportunities in the Central region.

5. **Plan for Seasonal Demand:** Use monthly sales trends to improve inventory planning, marketing campaigns, and sales strategies during high- and low-performing months.

6. **Understand Customer Segments:** Develop targeted marketing strategies based on customer segment purchasing behaviour.

## 10. Conclusion

This project demonstrates how Python can be used to perform Exploratory Data Analysis on retail sales data and extract meaningful business insights.

Through data cleaning, analysis, statistical exploration, and visualization, the project identified important trends in sales, profit, customer segments, product categories, regional performance, and discount sensitivity.

The findings highlight opportunities to improve profitability, optimize discount strategies, and support better business decisions through data-driven analysis.

## 11. How to Run the Project

Follow these steps to run the project on your local machine.

**Step 1: Clone the repository**

```bash
git clone <your-github-repository-url>
```

**Step 2: Navigate to the project directory**

```bash
cd Superstore-Sales-Analysis
```

**Step 3: Install the required libraries**

```bash
pip install pandas matplotlib seaborn openpyxl jupyter
```

**Step 4: Open Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5: Run the notebook**

Open `Superstore_Sales_Analysis.ipynb` and execute the notebook cells sequentially.

**Note:** Keep the dataset file `superstore_sales.csv.xlsx` in the same project directory as the notebook. The filename must match the filename used in the notebook's data-loading code.

## 12. Project Structure

```text
Superstore-Sales-Analysis/
│
├── Superstore_Sales_Analysis.ipynb
│
├── superstore_sales.csv.xlsx
│
└── README.md
```

## 13. Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Data Manipulation using Pandas
- Data Visualization using Matplotlib and Seaborn
- Statistical Analysis
- Correlation Analysis
- Outlier Detection
- Business Insight Generation
- Data-Driven Decision Making
