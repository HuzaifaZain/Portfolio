#  Housing Data Analytics Project

## Project Overview

This project demonstrates a **complete end-to-end data analytics lifecycle** applied to a housing dataset, starting from raw data ingestion to advanced data modeling and business-focused visualization. The primary aim was to transform an **unstructured, single flat source table** into a **clean, optimized, and scalable analytical model** that reflects **industry-standard BI practices**.

The project emphasizes **data modeling, performance optimization, and business insight generation**, making it highly relevant for real-world analytics, BI, and data analyst roles.

---

##  Business Problem Statement

Housing data is often provided in flat files with:

* Redundant and repetitive attributes
* No clear separation between descriptive and transactional data
* Poor performance during analysis
* Limited scalability for future data growth

This project addresses these challenges by:

* Designing a proper **star schema**
* Reducing data redundancy
* Improving analytical performance
* Creating KPIs that support **business and strategic decision-making**

---

##  Business Objectives

* Prepare raw housing data for enterprise-level analytics
* Eliminate redundancy and improve data consistency
* Reduce dataset complexity without losing business meaning
* Build a reusable and scalable data model
* Develop KPIs aligned with real estate business use cases
* Enable fast, interactive, and insight-driven reporting

---

##  Raw Dataset Description

* **Source Type**: CSV / Excel (single table)
* **Initial Structure**: Flat table
* **Total Columns**: 45
* **Total Rows**: Multiple housing transaction records

### Key Challenges in Raw Data

* Repeating attributes (location, property type, seller info)
* Mixed categorical and numerical fields
* Inconsistent naming conventions
* Missing and null values
* No primary or foreign keys

---

##  Data Cleaning (Power Query)

A robust data cleaning process was implemented using **Power Query** to ensure data accuracy and reliability.

### Cleaning Steps Performed

* Removed duplicate records
* Handled missing values using:

  * Logical imputation
  * Conditional replacements
  * Removal of non-business-critical null rows
* Standardized text fields:

  * Trimmed extra spaces
  * Unified capitalization
  * Corrected inconsistent spellings
* Converted and validated data types:

  * Dates
  * Currency values
  * Numerical measures
* Renamed columns using clear, business-friendly names
* Validated extreme values and outliers

---

##  Data Transformation

Data transformation was applied to make the dataset analytically meaningful.

### Key Transformations

* Derived new columns:

  * Property Age
  * Price per Unit Area
  * Price Bands
* Categorized continuous variables for segmentation
* Created conditional columns for business logic
* Ensured consistency across related attributes

---

##  Data Modeling Strategy

###  Modeling Approach

A **Star Schema** was implemented to separate descriptive attributes from transactional data.

### Why Star Schema?

* Faster query performance
* Cleaner DAX calculations
* Improved scalability
* Easier business understanding

---

##  Dimension Table Design

From the single raw table, multiple **dimension tables** were created.

###  Property Dimension

Contains static property-related attributes:

* Property ID (Surrogate Key)
* Property Type
* Property Category
* Construction Type

###  Location Dimension

Captures geographical details:

* Location ID
* City
* Area
* Region
* Postal Code

###  Time Dimension

Enables time intelligence analysis:

* Date ID
* Full Date
* Year
* Quarter
* Month

###  Seller Dimension

Stores seller-related information:

* Seller ID
* Seller Type
* Ownership Category

###  Buyer / Transaction Dimension

Defines transaction characteristics:

* Buyer ID
* Buyer Type
* Transaction Mode

Each dimension table uses a **unique surrogate ID**, which is referenced in the Fact Table.

---

##  Fact Table Design

The Fact Table represents housing transactions and contains:

### Keys

* Property ID
* Location ID
* Date ID
* Seller ID
* Buyer ID

### Measures

* Sale Price
* Area Size
* Price per Unit Area
* Transaction Count

---

##  Column Reduction & Optimization

### Before Data Modeling

* Single table with **45 columns**

### After Data Modeling

* Fact Table with **15 columns**

### Optimization Benefits

* Reduced redundancy
* Improved memory usage
* Faster report performance
* Cleaner data relationships

---

##  Business KPIs & Metrics

The following KPIs were developed using **DAX**:

* Total Sales Value
* Average Property Price
* Median Property Price
* Price per Unit Area
* Total Transactions
* Sales Growth (MoM / YoY)
* Property Type Contribution (%)
* Location-wise Performance
* High-Value Property Identification

---

##  Data Visualization & Dashboards

Interactive dashboards were built to support business users.

### Analysis Views

* Market trends over time
* Regional performance comparison
* Property category analysis
* Price distribution insights

### Visuals Used

* KPI Cards
* Line Charts
* Bar Charts
* Donut Charts
* Dynamic slicers

---

##  Tools & Technologies

* Power BI Desktop
* Power Query (ETL)
* DAX (KPI & Measures)
* Excel / CSV (Data Source)

---

##  Key Learnings

* Real-world data modeling from raw datasets
* Importance of surrogate keys and dimensions
* Performance optimization in BI models
* Business-driven KPI development
* Analytical storytelling through dashboards

---

##  Future Enhancements

* Add forecasting models
* Integrate external datasets
* Automate refresh using Power BI Service
* Advanced time intelligence calculations

---

##  Author

**Huzaifa Zain**
Mechanical Engineer | Data Analytics & Business Intelligence
Power BI • Data Modeling • DAX • Data Visualization

---


