# 📊 Market Mindz – End-to-End Data Analytics & BI Project

## 📌 Project Overview

**Market Mindz Analytics** is a comprehensive **end-to-end data analytics and business intelligence project** focused on transforming raw, unstructured marketing and sales data into **actionable business insights**. The project demonstrates how a **single flat source table** with a high number of columns can be converted into a **clean, optimized, and scalable analytical model** using **industry-standard data modeling and BI practices**.

The key strength of this project lies in **data modeling, column reduction, performance optimization, and KPI-driven storytelling**, making it a strong portfolio project for **Data Analyst, BI Analyst, and Power BI Developer roles**.

---

## 🎯 Business Problem Statement

Market Mindz collects extensive data related to:

* Marketing campaigns
* Customer interactions
* Sales performance
* Channels and regions
* Time-based trends

Initially, all data existed in a **single flat table**, which caused:

* Redundant and repeated columns
* Poor performance during analysis
* Difficulty in creating reusable KPIs
* Limited scalability for future data growth

This project addresses these challenges by implementing a **proper star schema**, reducing column count, and building business-focused dashboards.

---

## 🎯 Business Objectives

* Clean and standardize raw marketing and sales data
* Reduce redundancy and improve data quality
* Convert a flat dataset into a scalable star schema
* Reduce the total number of columns from **45 to 15**
* Improve reporting performance and usability
* Develop meaningful business KPIs
* Enable data-driven marketing and sales decisions

---

## 🗂️ Raw Dataset Description

* **Source Type**: CSV / Excel
* **Initial Structure**: Single flat table
* **Initial Columns**: 45
* **Data Coverage**:

  * Campaign details
  * Customer attributes
  * Product and service information
  * Channel and region data
  * Dates, costs, and revenues

### Key Issues in Raw Data

* Repeating campaign, channel, and customer attributes
* Mixed descriptive and transactional fields
* Inconsistent naming and formatting
* Missing and null values
* No primary or foreign keys

---

## 🧹 Data Cleaning (ETL – Power Query)

Data cleaning was performed using **Power Query**, following real-world ETL best practices.

### Cleaning Steps

* Removed duplicate records
* Handled missing values using:

  * Logical imputation
  * Conditional replacements
  * Removal of non-critical null rows
* Standardized text fields:

  * Campaign names
  * Channel names
  * Region names
* Corrected inconsistent spellings
* Converted and validated data types:

  * Dates
  * Currency values
  * Numeric measures
* Renamed columns to business-friendly names

---

## 🔄 Data Transformation

Transformations were applied to enrich the dataset and prepare it for analytics.

### Key Transformations

* Created calculated columns:

  * Revenue
  * Marketing Cost
  * Profit
  * ROI
  * Conversion Rate
* Categorized continuous values:

  * Cost bands
  * Revenue segments
* Created conditional columns for campaign performance classification
* Prepared clean lookup tables for dimension creation

---

## 🧩 Data Modeling Strategy

### ⭐ Modeling Approach

A **Star Schema** data model was implemented to clearly separate **facts** from **dimensions**.

### Why Star Schema?

* Faster report and query performance
* Simpler and more efficient DAX calculations
* Reduced redundancy
* Easy scalability for future datasets

---

## 📐 Dimension Tables Created

Multiple **dimension tables** were derived from the single source table.

### 1️⃣ Campaign Dimension

* Campaign ID (Surrogate Key)
* Campaign Name
* Campaign Type
* Start Date
* End Date

### 2️⃣ Customer Dimension

* Customer ID
* Customer Segment
* Customer Type

### 3️⃣ Channel Dimension

* Channel ID
* Marketing Channel
* Platform

### 4️⃣ Product / Service Dimension

* Product ID
* Product Category
* Service Type

### 5️⃣ Time Dimension

* Date ID
* Date
* Year
* Quarter
* Month

Each dimension table was assigned a **unique surrogate ID**, which replaced repetitive descriptive columns in the Fact Table.

---

## 📊 Fact Table Design

The **Marketing & Sales Fact Table** stores transactional and performance metrics.

### Keys

* Campaign ID
* Customer ID
* Channel ID
* Product ID
* Date ID

### Measures

* Impressions
* Clicks
* Conversions
* Revenue
* Cost
* Profit

---

## 📉 Column Reduction & Optimization

### Before Data Modeling

* Single flat table with **45 columns**

### After Data Modeling

* Optimized fact table with **15 columns**

### How Column Reduction Was Achieved

* Moved descriptive attributes into dimension tables
* Replaced repeated text columns with **dimension table IDs**
* Established one-to-many relationships using surrogate keys

### Benefits

* Reduced memory footprint
* Improved refresh and query performance
* Cleaner relationships
* Easier maintenance and scalability

---

## 📈 Business KPIs Developed

The following KPIs were developed using **DAX**:

* Total Revenue
* Total Marketing Cost
* Total Profit
* Return on Investment (ROI)
* Conversion Rate
* Cost per Conversion
* Revenue by Campaign
* Channel-wise Performance
* Customer Segment Contribution
* Campaign Performance Trend Over Time

---

## 📊 Data Visualization & Dashboards

Interactive dashboards were created to support marketing and business stakeholders.

### Dashboard Insights

* Campaign performance comparison
* ROI and profitability analysis
* Channel effectiveness
* Customer segmentation insights
* Trend analysis over time

### Visuals Used

* KPI Cards
* Line Charts
* Bar Charts
* Donut Charts
* Tables and matrices
* Interactive slicers

---

## 🚀 Tools & Technologies

* Power BI Desktop
* Power Query (ETL)
* DAX (Measures & KPIs)
* Excel / CSV (Data Source)

---

## 📌 Key Learnings & Outcomes

* Designed a full star schema from raw marketing data
* Reduced columns from **45 to 15** through proper modeling
* Improved BI performance and usability
* Developed business-focused KPIs
* Strengthened analytical storytelling skills

---

## 🔮 Future Enhancements

* Add predictive campaign performance analysis
* Integrate social media and digital analytics data
* Automate refresh using Power BI Service
* Implement advanced time intelligence KPIs

---

## 👤 Author

**Huzaifa Zain**
Data Analytics & Business Intelligence Enthusiast
Power BI • Data Modeling • DAX • Visualization

---

⭐ *If you find this project useful, feel free to star the repository!*

