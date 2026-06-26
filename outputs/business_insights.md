Task 3

# Business Insights – Calculated Fields

## Overview

The following calculated fields were created in Tableau to support business analysis and executive decision-making.

| Calculated Field | Tableau Formula | Business Purpose |
|------------------|-----------------|------------------|
| **Profit Margin** | `SUM([Profit]) / SUM([Sales])` | Measures the percentage of revenue retained as profit. Higher values indicate better profitability. |
| **Cost** | `SUM([Sales]) - SUM([Profit])` | Estimates the cost incurred to generate sales by subtracting profit from sales. |
| **Average Order Value** | `SUM([Sales]) / COUNTD([Order ID])` | Calculates the average revenue earned from each order, helping evaluate customer purchasing behavior. |
| **Return Rate** | `SUM([Return Flag]) / COUNTD([Order ID])` | Measures the proportion of returned orders relative to the total number of unique orders. |
| **Shipping Delay Bucket** | `IF [Delivery Days] <= 2 THEN "Fast Delivery" ELSEIF [Delivery Days] <= 5 THEN "Standard Delivery" ELSE "Delayed Delivery" END` | Categorizes deliveries into Fast, Standard, and Delayed groups for shipping performance analysis. |

---

## Business Interpretation

### Profit Margin

Profit Margin measures how efficiently the business converts sales into profit. A higher profit margin indicates stronger financial performance and better cost management.

### Cost

Cost estimates the expenses incurred to generate sales by subtracting profit from sales. This metric helps evaluate operational efficiency and profitability.

### Average Order Value

Average Order Value represents the average revenue earned from each customer order. It helps assess customer purchasing behavior and supports pricing and marketing strategies.

### Return Rate

Return Rate measures the percentage of orders that are returned. Higher return rates may indicate product quality issues, customer dissatisfaction, or fulfillment problems.

### Shipping Delay Bucket

Shipping Delay Bucket classifies deliveries into **Fast Delivery**, **Standard Delivery**, and **Delayed Delivery** based on the number of delivery days. This categorization helps monitor logistics performance and identify opportunities to improve delivery efficiency.

---

## Summary

These calculated fields provide the foundation for the executive dashboard by enabling profitability analysis, cost estimation, customer spending evaluation, return monitoring, and shipping performance assessment. Together, they support data-driven decision-making for retail leadership.

---

Task 8

# Business Insights

## Overview

The executive dashboard provides insights into sales performance, profitability, customer behavior, shipping efficiency, discount strategy, and return patterns. The following observations are based on the Tableau dashboard and the underlying dataset.

---

# Insight 1 – Sales Trend

### Observation
Sales remain relatively stable throughout the year, with noticeable peaks during **February** and **October**, while **April** records the lowest monthly sales.

### Data Evidence
- February Sales: **₹20.34 Million**
- October Sales: **₹19.84 Million**
- April Sales: **₹15.21 Million**

### Business Interpretation
Sales follow a seasonal pattern, indicating periods of stronger customer demand and periods of reduced purchasing activity.

### Recommended Action
Plan promotional campaigns and inventory replenishment before peak sales months and investigate factors contributing to lower sales in April.

---

# Insight 2 – Regional Performance

### Observation
The **South** region generates the highest sales and profit among all regions.

### Data Evidence
- South Sales: **₹64.69 Million**
- South Profit: **₹9.99 Million**
- South outperforms North, East, and West in both revenue and profitability.

### Business Interpretation
The South region is the strongest-performing market and contributes significantly to overall business performance.

### Recommended Action
Study successful sales strategies used in the South region and replicate them in lower-performing regions.

---

# Insight 3 – Category and Sub-Category Profitability

### Observation
The **Technology** category is substantially more profitable than the other product categories.

### Data Evidence
- Technology Profit: **₹28.04 Million**
- Furniture Profit: **₹3.56 Million**
- Office Supplies Profit: **₹1.71 Million**

Among sub-categories, **Copiers** generate the highest profit at approximately **₹7.31 Million**.

### Business Interpretation
Technology products provide the largest contribution to company profits, making them the primary profit driver.

### Recommended Action
Increase investment in Technology products while reviewing pricing and product mix for Furniture and Office Supplies to improve profitability.

---

# Insight 4 – Customer Segment Behavior

### Observation
The **Home Office** customer segment contributes the highest total sales.

### Data Evidence
- Home Office Sales: **₹74.50 Million**
- Consumer Sales: **₹71.89 Million**
- Corporate Sales: **₹70.63 Million**

### Business Interpretation
Home Office customers represent the most valuable customer segment in terms of revenue generation.

### Recommended Action
Develop targeted marketing campaigns and loyalty programs to retain Home Office customers while identifying opportunities to grow Corporate and Consumer sales.

---

# Insight 5 – Discount Impact

### Observation
Higher discount levels are associated with lower average profits, with profitability becoming negative at the highest discount level.

### Data Evidence
- 0% Discount Average Profit: **₹13,203**
- 25% Discount Average Profit: **₹3,113**
- 35% Discount Average Profit: **−₹1,601**

### Business Interpretation
Excessive discounting significantly reduces profitability and may lead to financial losses.

### Recommended Action
Review discount policies and limit high-discount promotions unless they are supported by increased sales volume or strategic objectives.

---

# Insight 6 – Shipping Performance

### Observation
Delivery time varies considerably across shipping modes.

### Data Evidence
Average Delivery Days:
- Same Day: **0.40 Days**
- First Class: **1.77 Days**
- Second Class: **2.68 Days**
- Standard Class: **4.71 Days**

### Business Interpretation
Premium shipping options provide significantly faster deliveries, while Standard Class has the longest delivery times.

### Recommended Action
Monitor Standard Class deliveries to identify operational improvements and encourage customers with urgent orders to select premium shipping options.

---

# Insight 7 – Return Pattern

### Observation
The **Furniture** category has the highest product return rate.

### Data Evidence
Return Rates:
- Furniture: **7.67%**
- Office Supplies: **3.65%**
- Technology: **3.03%**

The **East** region records the highest regional return rate at approximately **4.91%**.

### Business Interpretation
Furniture products are returned more frequently than other categories, suggesting potential issues related to product quality, customer expectations, or shipping.

### Recommended Action
Conduct a detailed analysis of Furniture returns to identify common causes and implement corrective actions such as quality improvements or enhanced product descriptions.

---

# Insight 8 – Business Risk and Opportunity

### Observation
The dashboard highlights a significant opportunity to increase profitability by combining strong-performing regions with high-margin product categories while controlling discounts and returns.

### Data Evidence
- Overall Sales: **₹217.02 Million**
- Overall Profit: **₹33.31 Million**
- Profit Margin: **15.35%**
- Technology is the highest-profit category.
- South is the highest-performing region.
- Furniture has the highest return rate.
- Discounts above 30% substantially reduce profitability.

### Business Interpretation
The business is financially healthy, but profitability can be further improved by focusing on high-performing regions and products while reducing unnecessary discounts and minimizing product returns.

### Recommended Action
Prioritize Technology product expansion in high-performing regions, optimize discount strategies, and implement return-reduction initiatives for Furniture products to maximize long-term profitability.

---

# Executive Summary

The dashboard indicates that the business maintains strong overall performance with **₹217.02 Million** in sales and a **15.35%** profit margin. Technology products and the South region are the primary contributors to profitability, while Furniture returns and aggressive discounting represent the greatest operational risks. By strengthening successful product lines, improving regional strategies, optimizing discounts, and reducing returns, leadership can further enhance revenue growth and overall profitability.