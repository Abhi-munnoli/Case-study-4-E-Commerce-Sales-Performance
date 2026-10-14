# 🛒 E-Commerce Sales Performance Analysis

### SwiftCart Retail Case Study | Python Data Analytics

## 📌 Project Overview

This project analyzes sales performance for SwiftCart, an e-commerce retailer selling Books, Clothing, Electronics, and Home products.

The analysis examines sales revenue, order quantities, product pricing, customer satisfaction, and premium-priced orders to identify business opportunities and potential risks.

Using Python and data visualization, this project demonstrates how sales data can be transformed into meaningful business insights to support product, inventory, and customer experience decisions.

## 🎯 Project Objectives

- Measure overall sales performance.
- Compare revenue and order quantities across product categories.
- Examine the distribution of product prices.
- Compare average customer ratings by category.
- Analyze the relationship between product price and customer rating.
- Identify potential risks associated with premium-priced orders.
- Develop data-driven business recommendations.

## 🗂️ Project Structure

```text
ecommerce-sales-performance-analysis/
│
├── README.md
├── E_Commerce_Sales_Performance.ipynb
├── ecommerce_sales_dataset.csv
└── ecommerce_sales_performance_report.pdf
```

## 📁 Dataset Description

The dataset contains **20 orders**, with Order IDs ranging from 1001 to 1020, across four product categories.

| Column | Description |
|---|---|
| `Order_ID` | Unique order identifier |
| `Product_Category` | Product category: Books, Clothing, Electronics, or Home |
| `Price` | Product price per order |
| `Quantity` | Number of units purchased |
| `Customer_Rating` | Customer rating on a scale of 1 to 5 |
| `Revenue` | Calculated as Price × Quantity |

The `Revenue` field is derived from price and quantity during the analysis.

## 🛠️ Technologies Used

- **Python** — Data analysis and calculations
- **Pandas** — Data manipulation, grouping, and aggregation
- **Matplotlib** — Data visualization
- **Jupyter Notebook** — Interactive analysis
- **Google Colab** — Cloud-based notebook execution
- **Data Formulator** — Charts and visual analysis, as documented in the report

## ⚙️ Analysis Workflow

### 1. Overall Sales Performance

Calculate total revenue, total units sold, average product price, and average customer rating.

Revenue is calculated using:

```python
df["Revenue"] = df["Price"] * df["Quantity"]
```

### 2. Category-Wise Revenue Analysis

Group orders by product category and compare total revenue, order counts, and units sold.

### 3. Product Price Distribution

Examine price ranges to understand where orders are concentrated and identify the distribution of lower- and higher-priced purchases.

### 4. Customer Satisfaction Analysis

Calculate average customer ratings by category to identify stronger-performing categories and those that may require further investigation.

### 5. Price vs. Customer Rating

Use correlation analysis and a scatter plot to examine whether higher prices are associated with higher customer ratings.

### 6. Premium-Order Risk Assessment

Identify the highest-priced 25% of orders using the report's price threshold of $3,176 and compare their revenue and average customer ratings with overall results.

## 📊 Key Findings

The following findings are taken from the accompanying PDF report.

### Overall Sales Performance

| Metric | Result |
|---|---:|
| Total orders | 20 |
| Total units sold | 61 |
| Total revenue | $143,323 |
| Average product price | $2,334.05 |
| Average customer rating | 3.86 / 5 |

### Revenue by Product Category

| Category | Orders | Units Sold | Total Revenue |
|---|---:|---:|---:|
| Home | 9 | 31 | $71,874 |
| Electronics | 6 | 16 | $38,910 |
| Clothing | 4 | 10 | $24,963 |
| Books | 1 | 4 | $7,576 |

**Key insight:** Home generated the highest revenue, contributing approximately 50.1% of total revenue. Electronics ranked second.

### Product Price Distribution

| Price Range | Number of Orders |
|---|---:|
| Below $1,000 | 4 |
| $1,000–$1,999 | 3 |
| $2,000–$2,999 | 7 |
| $3,000–$3,999 | 6 |

**Key insight:** Thirteen of the 20 orders were priced between $2,000 and $3,999, indicating that the sample is concentrated in the middle-to-high price ranges.

### Average Customer Rating by Category

| Category | Average Rating |
|---|---:|
| Home | 4.03 / 5 |
| Books | 
