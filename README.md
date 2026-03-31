# Olist E-commerce Analytics Dashboard

## Overview

This project analyzes an e-commerce dataset to track business performance across sales, customers, delivery operations, and payments. The objective is to convert raw transactional data into actionable insights using SQL and Power BI.

---

## Dataset

The project uses the Olist E-commerce dataset, which contains multiple related tables such as:

* Orders
* Order Items
* Customers
* Products
* Sellers
* Payments
* Reviews
* Category Translation

---

## Tech Stack

* PostgreSQL
* Power BI
* SQL
* DAX
* DirectQuery

---

## Data Pipeline

### 1. Database Setup

* Created a PostgreSQL database (`olist_db`)
* Designed raw tables for all dataset files

### 2. Data Loading & Validation

* Imported CSV data using COPY / pgAdmin
* Performed validation checks:

  * Row counts
  * Null values
  * Key column uniqueness

### 3. Data Modeling

* Built optimized SQL views for analysis
* Added indexes on frequently used columns:

  * `order_id`, `customer_id`, `product_id`, `seller_id`
* Structured data to support efficient joins and aggregation

### 4. Power BI Integration

* Connected PostgreSQL using DirectQuery
* Loaded only analytical views instead of raw tables
* Created a Date table for time-based analysis
* Established relationships between tables

---

## Key Metrics

* Revenue
* Orders
* Customers
* Average Order Value (AOV)
* Year-over-Year Growth (YoY %)
* On-time Delivery %
* Average Rating
* Payment Value

---

## Key Insights

* A small number of categories contribute a large share of total revenue
* Delivery delays are associated with lower customer ratings
* Certain regions show high sales volume along with higher delay rates
* Installment-based payments are commonly used for higher-value orders
* Revenue trends vary across months, indicating seasonal patterns

---

## Dashboard

The dashboard is divided into multiple pages:

* **Overview**
![Overview](PNG/Olist_(Overview).png)
  
* **Customer Insights**
![Customer Insights](PNG/Olist_(Customer).png)
  
* **Seller Insights**
![Seller Insights](PNG/Olist_(Seller).png)
  
* **Drillthrough**
![Drillthrough](PNG/Olist_(Drillthrough).png)
