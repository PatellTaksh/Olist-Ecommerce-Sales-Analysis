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

## Dashboard

The Power BI report is organized into multiple pages:

### Overview

* KPI cards: Revenue, Orders, Customers, AOV, YoY %, On-time %, Avg Rating
* Revenue trend over time
* Top categories by revenue
* Revenue distribution by state
* Order status breakdown

### Sales Trends

* Revenue vs previous year
* Rolling 30-day revenue
* Year-to-date performance
* Category-wise monthly matrix

### Category & Product

* Category contribution to revenue
* Orders vs AOV comparison
* Top categories by rating

### Customer Geography

* Revenue by state and city
* Top-performing regions
* State vs category performance

### Delivery & Logistics

* On-time delivery percentage
* Late order trends
* Delivery performance by region and category

### Reviews

* Rating distribution
* Positive vs negative review share
* Category-wise ratings

### Payments

* Payment method distribution
* Installment trends
* Payment value over time

### Sellers

* Total sellers and revenue per seller
* Top sellers by revenue
* Regional seller performance

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
![Overview](https://spbjhmjozqtxowgfyeht.supabase.co/storage/v1/object/public/images/dd33122c-791c-456e-8bdc-c20f1b853b87/1774947031625-8zmmpjxo3.png)
  
* **Customer Insights**
![Customer Insights](https://spbjhmjozqtxowgfyeht.supabase.co/storage/v1/object/public/images/dd33122c-791c-456e-8bdc-c20f1b853b87/1774947019347-5vxkp4fou.png)
  
* **Seller Insights**
![Seller Insights](https://spbjhmjozqtxowgfyeht.supabase.co/storage/v1/object/public/images/dd33122c-791c-456e-8bdc-c20f1b853b87/1774947040494-te25d5ahk.png)
  
* **Drillthrough**
![Drillthrough](https://spbjhmjozqtxowgfyeht.supabase.co/storage/v1/object/public/images/dd33122c-791c-456e-8bdc-c20f1b853b87/1774947026250-o76oyu49t.png)
