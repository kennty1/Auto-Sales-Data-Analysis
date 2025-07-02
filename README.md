# Auto-Sales-Data-Analysis
## Table of Contents
+ [Project Overview](#Project-Overview)
+ [Dataset Description](#Dataset-Description)
+ [Objectives](#Objectives)
+ [Tools Used](#Tools-Used)
+ [Analysis and Insight](#Analysis-and-Insight)   
  1. [Excel Dashboard](#excel-dashboard)
2.[SQL Queries](#sql-queries)
3.[PowerBi Dashboard](#PowerBi-Dashboard)
+ [Findings](#Findings)
---
## Project Overview
#### This Project analyses the Auto Sales Data which appears to be used for tracking sales performance and customer distribution across different regions, with most orders marked as "Shipped" and originating from multiple countries including the USA, France, and Australia.
---

## Data Description
|  Column            | Description                                                                    |
| ------------------ | ------------------------------------------------------------------------------ |
| `ORDERNUMBER`      | Unique identifier for each order.                                              |
| `QUANTITYORDERED`  | Number of items ordered.                                                       |
| `PRICEEACH`        | Price per item sold.                                                           |
| `ORDERLINENUMBER`  | Line number of the product in the order (used for multi-line orders).          |
| `SALES`            | Total revenue generated from the order line (PRICEEACH × QUANTITYORDERED).     |
| `ORDERDATE`        | Date the order was placed.                                                     |
| `DAYS_SINCE`       | Number of days since the order was made (likely relative to a reference date). |
| `STATUS`           | Order status (e.g., *Shipped*, *Disputed*).                                    |
| `PRODUCTCODE`      | Product identifier code.                                                       |
| `PRODUCTLINE`      | Product category (e.g., *Motorcycles*).                                        |
| `MSRP`             | Manufacturer's Suggested Retail Price.                                         |
| `CUSTOMERNAME`     | Name of the customer who placed the order.                                     |
| `PHONE`            | Customer phone number.                                                         |
| `ADDRESSLINE1`     | Primary customer address.                                                      |
| `CITY`             | City of the customer.                                                          |
| `POSTALCODE`       | Customer's postal code.                                                        |
| `COUNTRY`          | Country of the customer.                                                       |
| `CONTACTLASTNAME`  | Customer's last name.                                                          |
| `CONTACTFIRSTNAME` | Customer's first name.                                                         |
| `CONTACTFULLNAME`  | Full name of the customer (concatenated first and last names).                 |

---
## Objectives
+ Analyze Sales Performance:
   Evaluate total sales across different products, regions, and time periods to understand revenue patterns and top-performing items.
+ Track Customer Orders:
   Monitor customer behavior, order frequency, and volume to identify loyal customers and potential market segments.
+ Assess Product Demand:
   Determine which products (e.g., motorcycles) are most frequently ordered, at what price points, and in which regions.
+ Monitor Order Statuses:
   Examine the distribution of order statuses (e.g., *Shipped*, *Disputed*) to assess delivery performance and potential bottlenecks.
+ Geographic Insights:
   Map out customer locations by city and country to identify key markets and plan for regional marketing strategies.
+ Business Decision Support:
   Provide actionable insights to help managers make data-driven decisions regarding inventory, pricing, and customer service.
---
## Tools Used
+ MICROSOFT EXCEL
+ POWER BI
+ SQL
---
# Analysis and Insight 
## 1.Excel Dashboard
#### https://ibb.co/7t7t5QbM

## 2.SQL Queries
#### ---- THE HIGHEST QUANTITY OF GOODS ORDERED---
SELECT TOP 1 * FROM [dbo].[Auto Sales data]
ORDER BY QUANTITYORDERED DESC;

#### ---- THE LOWEST QUANTITY OF GOODS ORDERED---
SELECT TOP 1 * FROM [dbo].[Auto Sales data]
ORDER BY QUANTITYORDERED ASC;

#### --- ALL PRODUCTLINE---
SELECT PRODUCTLINE FROM [dbo].[Auto Sales data]
GROUP BY PRODUCTLINE;


#### --- CONTACT FULL NAME WITH SALES FROM HIGHEST  TO LOWEST----
SELECT CONTACTFULLNAME,MIN(SALES) FROM [dbo].[Auto Sales data]
group by CONTACTFULLNAME
ORDER BY CONTACTFULLNAME DESC;
---

## 3.Power Bi Dashboard
#### https://ibb.co/zTPXDVGr
#### https://ibb.co/g2hsHt3
---
# Findings
### 1. Most Orders Are Shipped:
   The majority of the orders in the dataset have a status of "Shipped", indicating a high fulfillment rate and good operational flow.
### 2. Popular Product Line – Motorcycles:
   All visible entries are from the Motorcycle product line, suggesting that this product category may be a major revenue driver.
### 3. Order Volumes Vary:
   The quantity ordered ranges from small (e.g., 1 unit) to larger bulk orders (up to 66 units), indicating a mix of retail and possible wholesale transactions.
### 4. Sales Values Differ Widely:
   The sales amounts (total revenue per order line) vary significantly, showing different pricing tiers and customer spending levels.
### 5. Geographically Diverse Customers:
   Customers are located in various countries including the **USA, France, Australia, UK, Norway, and Spain**, highlighting an international customer base.
### 6. Active Customer Engagement:
   Each record contains full contact information (phone, address, and names), suggesting that the company maintains detailed CRM (Customer Relationship Management) records.
### 7. Recent Sales Activity:
   Many order dates fall in 2020, showing relatively recent business activity and suggesting the data is used for current performance monitoring.




