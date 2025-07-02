# Auto-Sales-Data-Analysis

|  Column            | Description                                                                  |
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
