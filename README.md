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
| Books | 3.80 / 5 |
| Electronics | 3.73 / 5 |
| Clothing | 3.65 / 5 |

**Key insight:** Home achieved the highest average customer rating, while Clothing recorded the lowest average rating in the sample.

### Price and Customer Satisfaction

- **Price-rating correlation:** -0.23
- **Interpretation:** The report identifies a weak negative relationship between price and customer rating.

Higher-priced products did not consistently receive higher ratings in this sample. Price alone should therefore not be treated as a reliable indicator of customer satisfaction.

### Premium-Order Risk Analysis

| Metric | Result |
|---|---:|
| Premium-price threshold | $3,176 and above |
| Premium-priced orders | 5 |
| Premium-order revenue | $51,344 |
| Average premium-order rating | 3.04 / 5 |
| Overall average customer rating | 3.86 / 5 |

**Key insight:** The five premium-priced orders generated meaningful revenue, but their average customer rating was lower than the overall average. This warrants further investigation into product quality, value perception, product descriptions, and customer service.

## 💡 Business Recommendations

1. **Prioritize Home products:** Review inventory availability and maintain stock for products contributing strongly to revenue and customer satisfaction.
2. **Investigate Electronics feedback:** Examine customer ratings and product-level feedback to identify opportunities to improve satisfaction.
3. **Review Clothing performance:** Investigate the category's relatively low average rating before making major inventory decisions.
4. **Evaluate premium-priced orders:** Review customer feedback and product quality for expensive orders with lower ratings.
5. **Avoid price-only decisions:** Consider revenue, quantity, and customer satisfaction together when evaluating products.
6. **Expand the dataset:** Analyze more orders and additional attributes to support stronger commercial decisions.

## 📈 Visualizations

The accompanying analysis report includes:

- Revenue comparison across product categories.
- Histogram of product prices.
- Average customer ratings by category.
- Scatter plot of product price versus customer rating.

These visualizations help compare business performance and identify patterns that may require further investigation.

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `E_Commerce_Sales_Performance.ipynb`.
3. Upload `ecommerce_sales_dataset.csv` when required.
4. Run the notebook cells sequentially.
5. Review the analysis outputs and visualizations.

### Option 2: Run Locally

**Step 1 — Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/ecommerce-sales-performance-analysis.git
```

**Step 2 — Open the project directory**

```bash
cd ecommerce-sales-performance-analysis
```

**Step 3 — Install the required libraries**

```bash
pip install pandas matplotlib jupyter
```

**Step 4 — Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `E_Commerce_Sales_Performance.ipynb` and execute the cells.

**Note:** Ensure the notebook reads `ecommerce_sales_dataset.csv` from the project directory. Update any file paths or Google Colab-specific upload code if necessary.

## 📄 Project Report

The `ecommerce_sales_performance_report.pdf` file contains the detailed case study, including:

- Introduction, problem statement, and objectives.
- Dataset description and tools used.
- Overall sales performance.
- Category-wise revenue and quantity analysis.
- Product price distribution.
- Customer satisfaction comparisons.
- Price-rating relationship.
- Premium-order risk assessment.
- Key findings, recommendations, and conclusion.

## ⚠️ Limitations

- The dataset contains only 20 orders.
- The findings describe the supplied sample and may not represent overall business performance.
- The analysis does not include product costs, profit margins, or marketing expenses.
- Correlation does not establish causation.
- Further order history and product-level details are needed before making major forecasting or inventory decisions.

## 🏁 Conclusion

The analysis shows that Home is the strongest-performing category under the selected revenue and customer satisfaction measures. However, premium-priced orders have a lower average customer rating than the overall sample, highlighting a potential area for further investigation.

SwiftCart can use these descriptive findings to guide inventory reviews, customer satisfaction improvements, and premium-product evaluations. A larger dataset would help validate these patterns and support more reliable business decisions.

## 👨‍💻 Author

**Abhinandan Babu Munnoli**

Aspiring AI & Machine Learning Engineer | Python Developer | Final-Year Computer Science Engineering Student

- **GitHub:** [Abhi-munnoli](https://github.com/Abhi-munnoli)
- **LinkedIn:** [Connect with me](https://www.linkedin.com/in/abhinandan-munnoli-361a932bb/)

---

⭐ If you find this project useful, consider giving the repository a star.

*Developed as an educational e-commerce sales analytics case study.*
