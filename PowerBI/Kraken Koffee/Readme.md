# ☕ Kraken Koffee – End-to-End Data Analytics Project

## 📌 Project Overview

**Kraken Koffee Analytics** is an end-to-end **business intelligence and data analytics project** designed to analyze sales, customer behavior, product performance, and operational trends for a fictional coffee business, *Kraken Koffee*.

The project demonstrates how a **single raw transactional dataset** can be transformed into a **clean, optimized, and scalable analytical data model** using **industry-standard BI practices**. The focus is not only on visuals, but on **strong data modeling, performance optimization, and business-driven KPIs**.

This project is built as a **portfolio-grade BI solution**, suitable for real-world business analytics, Power BI development, and data analyst roles.

---

## 🎯 Business Problem Statement

Kraken Koffee generates large volumes of transactional data related to:

* Sales
* Products
* Customers
* Stores
* Time

However, the raw data exists as a **single flat table**, which:

* Contains repeated attributes
* Is difficult to scale
* Performs poorly for analytics
* Makes KPI development complex

This project solves these challenges by:

* Designing a **star schema data model**
* Reducing redundancy using **dimension tables**
* Creating business-ready KPIs
* Delivering interactive dashboards for decision-makers

---

## 🎯 Business Objectives

* Convert raw sales data into analytics-ready format
* Reduce column redundancy and improve performance
* Implement proper data modeling (Fact & Dimensions)
* Enable slicing and dicing by product, store, customer, and time
* Develop KPIs for sales, profitability, and operations
* Support data-driven decision-making

---

## 🗂️ Raw Dataset Description

* **Source Type**: CSV / Excel
* **Structure**: Single flat transactional table
* **Initial Columns**: High number of mixed attributes
* **Data Includes**:

  * Order details
  * Product information
  * Customer details
  * Store/location data
  * Dates and pricing

### Key Issues in Raw Data

* Repeating product and store attributes
* No separation between descriptive and transactional data
* Inconsistent text formatting
* Missing and null values
* No primary or foreign key structure

---

## 🧹 Data Cleaning (ETL Process)

Data cleaning was performed using **Power Query** to ensure data accuracy and consistency.

### Cleaning Steps

* Removed duplicate transaction records
* Handled missing values using:

  * Conditional replacement
  * Logical imputation
  * Removal of non-critical null records
* Standardized text fields:

  * Product names
  * Store names
  * Customer categories
* Corrected inconsistent spellings
* Converted data types:

  * Dates
  * Currency values
  * Numerical measures
* Renamed columns for clarity and business readability

---

## 🔄 Data Transformation

Transformations were applied to enrich the dataset and make it suitable for analysis.

### Key Transformations

* Created calculated columns:

  * Revenue
  * Profit
  * Profit Margin (%)
  * Order Size
* Categorized continuous values:

  * Price bands
  * Order value segments
* Created conditional logic columns for business rules
* Prepared clean lookup tables for modeling

---

## 🧩 Data Modeling Strategy

### ⭐ Modeling Approach

A **Star Schema** was implemented to separate facts from dimensions, following best BI practices.

### Why Star Schema?

* Improved report performance
* Simpler DAX calculations
* Reduced data redundancy
* Better scalability and maintenance

---

## 📐 Dimension Tables Created

Multiple **dimension tables** were created from the single source table.

### 1️⃣ Product Dimension

Contains all product-related attributes:

* Product ID (Surrogate Key)
* Product Name
* Category
* Size
* Cost

### 2️⃣ Customer Dimension

Stores customer information:

* Customer ID
* Customer Type
* Loyalty Segment

### 3️⃣ Store Dimension

Captures store-level details:

* Store ID
* Store Name
* City
* Region

### 4️⃣ Time Dimension

Enables time intelligence analysis:

* Date ID
* Date
* Year
* Month
* Quarter
* Day

Each dimension table uses a **unique surrogate ID**, which is referenced in the Fact Table.

---

## 📊 Fact Table Design

The **Sales Fact Table** stores transactional metrics.

### Keys

* Product ID
* Customer ID
* Store ID
* Date ID

### Measures

* Quantity Sold
* Revenue
* Cost
* Profit

---

## 📉 Column Reduction & Optimization

### Before Modeling

* Single flat table with a large number of columns

### After Modeling

* Optimized fact table with significantly fewer columns

### How Column Reduction Was Achieved

* Moved descriptive attributes into dimension tables
* Replaced repeated text columns with **dimension IDs**
* Maintained relationships using surrogate keys

### Benefits

* Reduced memory usage
* Faster report refresh and interaction
* Cleaner data relationships
* Improved model scalability

---

## 📈 Business KPIs Developed

The following KPIs were created using **DAX**:

* Total Revenue
* Total Profit
* Profit Margin (%)
* Total Orders
* Average Order Value (AOV)
* Revenue by Product Category
* Top Performing Stores
* Customer Segment Contribution
* Sales Trend Over Time

---

## 📊 Data Visualization & Dashboards

Interactive dashboards were built to support business users.

### Dashboard Insights

* Sales and profit trends over time
* Product category performance
* Store-wise revenue comparison
* Customer segmentation analysis
* High-margin vs low-margin products

### Visuals Used

* KPI Cards
* Line Charts
* Bar Charts
* Donut Charts
* Tables and matrices
* Slicers for dynamic filtering

---

## 🚀 Tools & Technologies

* Power BI Desktop
* Power Query (ETL)
* DAX (Measures & KPIs)
* Excel / CSV (Data Source)

---

## 📌 Key Learnings

* Designed a complete star schema from raw transactional data
* Implemented surrogate keys and dimension modeling
* Improved BI performance through column reduction
* Developed business-driven KPIs
* Strengthened data storytelling skills

---

## 🔮 Future Enhancements

* Add forecasting and trend analysis
* Integrate inventory data
* Automate refresh using Power BI Service
* Implement advanced time intelligence KPIs

---

## 👤 Author

**Huzaifa Zain**
Data Analytics & Business Intelligence Enthusiast
Power BI • Data Modeling • DAX • Visualization

---

⭐ *If you find this project useful, feel free to star the repository!*

