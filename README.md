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
#### https://ibb.co/pvsTBPvH

## 2.SQL Queries
#### https://ibb.co/CpWj0mjK

## 3.Power Bi Dashboard
#### https://ibb.co/QvszvFk3
---
# Findings
 ### 1. Majority Education Level: Most employees have a Bachelors degree.
### 2. Common Cities: The majority of employees are located in Bangalore, followed by Pune and New Delhi.
### 3. Payment Tier Distribution: Most employees are in PaymentTier 3, indicating a concentration in the highest pay level.
### 4. Age Range: Employees' ages range from early 20s to late 30s, with many in their 30s.
### 5. Gender Representation: The dataset includes both Male and Female employees, with a slight male majority.
### 6. Experience Levels: Experience varies widely, from 0 to 5 years prior to joining.
### 7. Employee Attrition (LeaveOrNot): There are both leavers (`1`) and stayers (`0`), allowing for predictive modeling on attrition behavior.


