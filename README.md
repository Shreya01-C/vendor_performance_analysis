# Venor Parfomance Analysis
## Overview
-
This project evaluates vendor performance and retail inventory dynamics to drive strategic insights for purchasing, pricing, and inventory optimization. A complete data pipeline was built using SQL for ETL, Python for analysis and hypothesis testing, and Power BI for visualization.
---
## Business Problem
Effective inventory and sales management are critical in the retail sector. This project aims to:
- Identify underperforming brands needing pricing or promotional adjustments
- Determine vendor contributions to sales and profits
- Analyze the cost-benefit of bulk purchasing
- Investigate inventory turnover inefficiencies
- Statistically validate differences in vendor profitability
--- 
## Tools & Technologies
- SQL 
- Python 
- Power BI 
---
## Data Cleaning & Preparation
-
Removed transactions with:
Gross Profit ≤ 0
Profit Margin ≤ 0
Sales Quantity = 0
Created summary tables with vendor-level metrics
Converted data types, handled outliers, merged lookup tables
--- 
## Exploratory Data Analysis (EDA)
### Negative or Zero Values Detected:
- Gross Profit: Min -52,002.78 (loss-making sales)
- Profit Margin: Min -∞ (sales at zero or below cost)
- Unsold Inventory: Indicating slow-moving stock

### Outliers Identified:
- High Freight Costs (up to 257K)
- Large Purchase/Actual Prices

### Correlation Analysis:
- Weak between Purchase Price & Profit
- Strong between Purchase Qty & Sales Qty (0.999)
- Negative between Profit Margin & Sales Price (-0.179)

---
## Dashboard
Power BI Dashboard shows:
- Vendor-wise Sales and Margins
- Inventory Turnover
- Bulk Purchase Savings
- Performance Heatmaps
- Vendor Performance Dashboard
---
## Final Recommendations
- Diversify vendor base to reduce risk
- Optimize bulk order strategies
- Reprice slow-moving, high-margin brands
- Clear unsold inventory strategically
- Improve marketing for underperforming vendors
