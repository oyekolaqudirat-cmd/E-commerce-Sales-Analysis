# E-commerce-Sales-Analysis
The analysis aims to uncover patterns in sales performance, identify high- and low-performing products, understand customer return behaviour, and evaluate payment outcomes. The findings can help the business identify operational challenges, understand its performance drivers, and make more informed, data-driven decisions.
# E-Commerce Data Analysis Using Python

**Revenue, Product Performance, Returns, and Payment Analysis**

## 1. Project Overview

This project analyzes e-commerce data using Python to evaluate business performance across four key areas: revenue, product performance, returns, and payment transactions.

The goal is to identify sales trends, evaluate product performance, understand customer return behavior, and assess payment outcomes. The findings provide insights into business performance and highlight areas that may require operational improvement.

### Tools and Data Source

The data was gotten from chatgpt
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## 2. Business Problem

The business generates data from sales orders, products, payments, and product returns but needs a clearer understanding of what the data reveals about its overall performance.

Without structured analysis, it may be difficult to determine which products contribute most to revenue, which periods experience high or low sales, which products have elevated return rates, or whether payment failures and pending transactions indicate operational issues.

This project addresses these challenges by analyzing four datasets and translating the results into business insights and recommendations.

## 3. Project Objectives

- Evaluate overall revenue performance and identify monthly and yearly sales trends.
- Analyze average order value (AOV) and customer spending patterns.
- Investigate the relationship between discounts and revenue over time.
- Identify high- and low-performing products and categories.
- Examine product return rates, reasons, and patterns.
- Assess payment outcomes, including successful, failed, pending, and refunded transactions.
- Identify data-quality issues and potential inconsistencies in business records.
- Develop evidence-based recommendations to support business decision-making.

## 4. Data Preparation and Quality Assessment

Before conducting the analysis, the datasets were reviewed and prepared to improve data quality and reliability.

The data preparation process involved examining:

- Data types and date formats
- Missing values
- Duplicate records
- Inconsistent categorical values
- Invalid values and potential outliers
- Potential inconsistencies between orders, returns, and payments

The prepared data was organized into four analytical datasets:

1. Revenue Analysis
2. Product Analysis
3. Returns Analysis
4. Payment Analysis

Each dataset was analyzed independently to address its relevant business questions.

## 5. Analysis and Key Findings

### 5.1 Revenue Analysis

**Objective:** Evaluate sales performance, understand revenue trends, and investigate customer spending and discount patterns.

#### Key Findings

| Metric | Result |
|---|---:|
| Total Revenue | 2,720,985,600 |
| Average Order Value | 159,475 |
| Average Revenue per Customer | 566,400 |
| Highest-Revenue Month | October |
| October Revenue | Over 233,157,000 |
| Lowest-Revenue Month | February |
| February Revenue | 202,195,000 |

***Revenue Trend Over Time***
![Revenue Trend over the months](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Revenue%20Trend%20Over%20time.png)

#### Discount Analysis

- Low-discount transactions recorded the highest order volume.
- Medium-discount transactions generated the highest total discount amount.
- High-discount transactions recorded the lowest order volume and discount amount.

These findings indicate that order volume and discount levels should be evaluated together when assessing promotional performance.

#### Customer Segment Analysis

- New customers generated the highest revenue.
- Regular customers generated the lowest revenue.
- Customers with an unknown segment contributed the least revenue among the recorded segments.

The unknown segment requires further investigation to determine why these customers could not be classified

***Customer Segment***
![Customer Segment](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Customer%20Segment%20Sales.png)

#### Shipping Fee Analysis

- Low shipping fees recorded the highest order volume.
- Medium shipping fees generated the highest revenue.
- High shipping fees were associated with lower purchasing activity.

The business should investigate the relationship between shipping fees and purchasing behavior before changing its shipping strategy.

### 5.2 Product Analysis

**Objective:** Evaluate product and category performance to identify strong performers and products that may require further investigation.

#### Key Findings

| Metric | Result |
|---|---|
| Highest-Revenue Product | Vitamin C Serum |
| Vitamin C Serum Revenue | 63,200,518 |
| Lowest-Revenue Product | Gentle Cleanser 86 |
| Gentle Cleanser 86 Revenue | 2,967,526 |
| Best-Performing Category | Skincare |
| Highest-Margin Product | Gentle Cleanser 35 |
| Highest Profit Margin | 91.8% |

***Top 10 products***
![Top products](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Top%2010%20products.png)

#### Business Interpretation

Vitamin C Serum was the highest-revenue product, while Gentle Cleanser 86 recorded the lowest revenue among the products identified.

Skincare was the best-performing category. Gentle Cleanser 35 recorded the highest profit margin at 91.8%.

Revenue and profitability are different measures. A product with high revenue does not necessarily generate the highest profit.

### 5.3 Returns Analysis

**Objective:** Understand return activity and identify categories, products, and return reasons associated with higher return levels.

#### Key Findings

| Metric | Result |
|---|---:|
| Total Item Returns | 2,470 |
| Reported Return Rate | 15% |
| Approved Returns | 1,778 |
| Rejected Returns | 379 |
| Pending Returns | 297 |

#### Returns by Category

| Category | Recorded Returns |
|---|---:|
| Skincare | 1,618 |
| Accessories | 372 |
| Haircare | 550 |
| Bodycare | 550 |

***Return By Category***
![Return by Category](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Return%20per%20category.png)

#### Returns by Reason

| Return Reason | Count |
|---|---:|
| Damaged | 455 |
| Other | 415 |
| Quality Issue | 407 |
| Late Delivery | 407 |
| Wrong Item | 400 |
| Changed Mind | 386 |

#### Return Trends

- The highest-return quarter was Q3, with 636 returns.
- The lowest-return quarter was Q4, with 592 returns.
- The recorded biannual return volume was reported as 2,470.

  ***Return Trend***
  ![Return Trend](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Return%20trend%20over%20time.png)

  ***Return Status Distribution***
  ![Return Status Distribution](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Return%20status%20distribution.png)

#### Business Interpretation

Damaged products were the most frequently recorded return reason, followed by other reasons and quality issues.

The business should investigate product handling, packaging, quality control, and fulfilment processes to determine whether these factors contribute to returns.

Late deliveries and wrong-item returns also warrant attention because they may indicate operational or fulfilment challenges.

Return counts should be monitored consistently across categories, periods, and statuses to support reliable reporting.

### 5.4 Payment Analysis

**Objective:** Evaluate payment outcomes and identify potential issues in the transaction process.

#### Transaction Volume by Payment Status

| Payment Status | Transaction Count |
|---|---:|
| Successful | 14,388 |
| Pending | 1,517 |
| Failed | 1,462 |
| Refunded | 1,064 |
| Unknown | 9 |

#### Transaction Value by Payment Status

| Payment Status | Transaction Value |
|---|---:|
| Successful | 1,317,527,000 |
| Pending | 139,727,300 |
| Failed | 134,883,000 |
| Refunded | 97,513,260 |
| Unknown | 1,116,079 |

***Payment method by status***
![Payment method by status](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Payment%20method%20by%20status.png)

#### Payment Method Analysis

- Card payments recorded the highest reported failure rate at 8.19%.
- Bank transfers recorded the lowest reported failure rate at 7.4%.
- Card payments recorded a successful transaction rate above 78%.

#### Potential Order and Payment Inconsistency

A total of **1,405 records** had a cancelled order status despite indicating successful payment.

These records require further investigation to determine whether they represent payment-status synchronization issues, unprocessed cancellations, missing refunds, or other operational problems.

Payment attempts should be distinguished from distinct orders to avoid overstating order counts or assuming that every failed payment represents a lost sale.

## 6. Business Recommendations

### Sales and Revenue

- Monitor monthly and yearly revenue trends to identify peak and low-sales periods.
- Investigate factors associated with changes in revenue.
- Use customer spending patterns to identify opportunities for customer retention and increased customer value.

### Discount Strategy

- Evaluate discounts alongside order volume, units sold, average order value, and revenue.
- Compare performance across discount levels before changing promotional strategies.
- Avoid assuming that higher discounts automatically lead to higher revenue or profitability.

### Product Management

- Investigate the factors behind low revenue for underperforming products.
- Review high-performing products to understand their contribution to sales.
- Monitor profit margins alongside revenue where reliable cost data is available.

### Shipping Strategy

- Investigate the relationship between shipping fees and order volume.
- Evaluate whether high shipping fees contribute to reduced purchasing activity.
- Test alternative shipping strategies before substantially reducing or eliminating shipping charges.

### Returns Management

- Investigate damaged-product returns and review packaging and quality-control processes.
- Examine late deliveries and wrong-item returns to identify fulfilment issues.
- Monitor return rates by product and category using consistent denominators.
- Review pending and rejected returns to improve return-status management.

### Payment Operations

- Investigate the 1,405 cancelled-order records with successful payment statuses.
- Monitor failed and pending transactions by payment method.
- Review refund processing and payment-status synchronization.
- Distinguish payment attempts from distinct orders when calculating transaction metrics.

### Data Quality

- Maintain validation rules for revenue, orders, returns, and payment outcomes.
- Use consistent definitions for return counts and rates.
- Investigate discrepancies between overall return totals and period-based summaries.
- Ensure that cancelled orders, refunds, and repeated payment attempts are handled consistently.

## 7. Limitations

- The analysis depends on the completeness and accuracy of the available data.
- Some return summaries require further validation because their reported totals differ.
- Relationships between discounts, shipping fees, and sales do not establish causation.
- Return rates depend on a clearly defined order-based or item-based denominator.
- Payment attempts and distinct orders are not interchangeable.
- Profitability conclusions require reliable cost data.
- The causes of order and payment-status inconsistencies cannot be established from recorded statuses alone.

## 8. Conclusion

This project applied Python-based data analysis to examine e-commerce performance across revenue, products, returns, and payments.

The analysis identified revenue trends, customer spending patterns, high- and low-performing products, common return reasons, payment outcomes, and potential inconsistencies between order and payment records.

The findings highlight areas for further investigation, including shipping fees, product returns, payment failures, and cancelled orders with successful payment statuses.

The project demonstrates how Python can be used to transform raw operational data into meaningful insights that support sales planning, product management, returns handling, payment monitoring, and business decision-making.

## 9. Skills Demonstrated

- Data cleaning and validation
- Exploratory data analysis (EDA)
- Data aggregation and grouping
- Business metric calculation
- Time-based trend analysis
- Product and customer performance analysis
- Returns and payment analysis
- Data visualization
- Business interpretation and recommendation development
- Communicating analytical findings

## 10. Project Structure

```text
e-commerce-data-analysis/
│
├── data/
│   ├── revenue_analysis.csv
│   ├── product_analysis.csv
│   ├── returns_analysis.csv
│   └── payment_analysis.csv
│
├── notebooks/
│   └── ecommerce_analysis.ipynb
│
├── visuals/
│   └── charts_and_visualizations/
│
└── README.md
```

## 11. Python Code
[View the Complete Analysis Notebook](https://github.com/oyekolaqudirat-cmd/E-commerce-Sales-Analysis/blob/main/Sales_Project.ipynb)
