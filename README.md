Here is the complete, properly formatted README file, now including the repository structure to match your files. You can copy and paste this directly into your GitHub repository.

---

# Advanced Vendor Performance Analysis

## Overview

Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. This project provides an end-to-end data analytics solution to identify areas for improvement, ranging from underperforming brands to vendor dependency risks.

## Repository Structure

```text
├── Dashboard Preview.png
├── README.md
├── Vendor Performance Analysis.ipynb
├── Vendor Performance Report.pdf
├── Vendor-Performance-Analysis presentation pdf.pdf
├── Vendor-Performance-Analysis presentation pptx.pptx
├── Vendor_performance_Analysis.pbix
├── background.png
└── vendor_sales_summary.csv

```

## Tools & Technologies Used

* **Programming & EDA:** Python (Pandas for data manipulation and cleaning)
* **Visualization:** Matplotlib, Seaborn, Power BI (Dashboard creation)
* **Database Management:** SQLite
* **Data Pipeline:** Real-time data ingestion with logging

## Business Problem & Optimization Goals

The primary objectives of this analysis are to:

* **Identify Underperforming Brands:** Pinpoint brands requiring promotional or pricing adjustments.
* **Determine Top Vendors:** Recognize vendors contributing significantly to overall sales and gross profit.
* **Analyze Bulk Purchasing:** Assess the impact of large-quantity orders on unit cost savings.
* **Improve Inventory Turnover:** Reduce holding costs and enhance efficiency by identifying slow-moving stock.
* **Investigate Profitability Variance:** Compare performance metrics between high-performing and low-performing vendors.

## Data Processing & Filtering

To ensure the reliability of the insights, inconsistent data points were removed prior to analysis:

* Excluded transactions resulting in a Gross Profit of 0 or less to avoid factoring in losses.
* Excluded transactions with a Profit Margin of 0 or less to focus strictly on profitable items.
* Eliminated inventory with a Total Sales Quantity of 0 to remove stock that was purchased but never sold.

## Key Findings & Exploratory Data Analysis

### 1. Vendor Contribution & Dependency

* The top 10 vendors account for 65.69% of all purchases, while the remaining vendors make up only 34.31%.
* This high reliance on key vendors, such as DIAGEO NORTH AMERICA INC, Martignetti Companies, and Pernod Ricard USA, introduces potential supply chain risks.

### 2. Pricing & Promotional Opportunities

* The analysis identified 198 brands exhibiting lower sales volumes but higher profit margins.
* Brands like Crown Royal Apple (89.81% margin) and Concannon Glen Ellen Wh Zin (83.45% margin) present strong opportunities for targeted marketing and price optimizations to increase volume without sacrificing profitability.

### 3. Bulk Purchasing Impact

* Vendors purchasing in large quantities achieve a 72% lower unit cost, dropping to **$10.78** per unit compared to the higher costs associated with smaller orders.
* This indicates that bulk pricing strategies successfully encourage larger orders, increasing total sales while maintaining profitability.

### 4. Inventory Turnover & Inefficiencies

* There is **$2.71M** tied up in total unsold inventory capital.
* Vendors such as Alisa Carr Beverages and Highland Wine Merchants LLC show low inventory turnover, highlighting slow-moving stock that increases storage costs and reduces cash flow efficiency.

### 5. Profitability Variance

* Top-performing vendors maintain an average profit margin of **31.17%**.
* Low-performing vendors maintain a higher average profit margin of **41.55%**, yet struggle with overall sales volumes.
* Hypothesis testing confirmed a statistically significant difference in profit margins between these two groups, suggesting they operate under distinctly different profitability models.

## Dashboard Highlights

The project features a comprehensive Power BI dashboard summarizing overall operational performance:

* **Total Sales:** $441.41M
* **Total Purchase:** $307.34M
* **Gross Profit:** $134.07M
* **Top Selling Brands:** Jack Daniels, Tito's Handmade Vodka, and Grey Goose consistently lead the sales charts.

## Strategic Recommendations

* **Diversify Vendors:** Reduce dependency on the top few suppliers by adding medium-level partners to mitigate supply chain disruptions.
* **Improve Inventory Planning:** Increase stock levels for fast-selling brands and reduce purchase quantities for slow-moving inventory to avoid overstocking and wasted capital.
* **Optimize Pricing & Promotions:** Implement targeted discounts or better market positioning for the 198 low-sales, high-margin brands to drive higher volumes.
* **Leverage Bulk Purchasing:** Utilize performance data to negotiate better prices, discounts, or payment terms, taking full advantage of bulk purchasing savings.
* **Address Low Performers:** Enhance marketing efforts for low-performing vendors and consider product rationalization (reducing or removing items) if performance metrics do not improve.
