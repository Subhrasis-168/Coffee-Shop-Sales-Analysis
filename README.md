# ☕ Coffee Shop Sales Analytics

> An Excel-based data analytics project focused on analyzing coffee shop sales, transaction activity, product performance, store performance, and customer demand patterns.

[![Microsoft Excel](https://img.shields.io/badge/Microsoft%20Excel-Data%20Analytics-217346?logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/microsoft-365/excel)
[![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Subhrasis-168/Coffee-Shop-Sales-Analysis)

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Business Questions](#-business-questions)
- [Dataset](#-dataset)
- [Data Preparation](#-data-preparation)
- [Analysis Performed](#-analysis-performed)
- [Key Performance Indicators](#-key-performance-indicators)
- [Dashboard](#-dashboard)
- [Dashboard Features](#-dashboard-features)
- [Key Insights](#-key-insights)
- [Business Recommendations](#-business-recommendations)
- [Tools & Excel Techniques](#-tools--excel-techniques)
- [Project Workflow](#-project-workflow)
- [Repository Structure](#-repository-structure)
- [How to Use](#-how-to-use)
- [Project Outcomes](#-project-outcomes)
- [Skills Demonstrated](#-skills-demonstrated)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 📊 Project Overview

**Coffee Shop Sales Analytics** is a Microsoft Excel data analytics project built using coffee shop transaction data covering **January to June 2023**.

The project converts transaction-level sales data into an interactive Excel dashboard that helps analyze:

- Sales performance
- Transaction-based customer activity
- Average bill and order metrics
- Hourly order quantity
- Product category contribution
- Product size distribution
- Store-level performance
- Top-performing products
- Weekday transaction activity

The analysis contains **149,116 transactions** and uses additional analytical fields to support time-based analysis, grouping, filtering, PivotTable analysis, and dashboard visualization.

The objective is to transform detailed transactional data into a clear business reporting solution that makes sales and customer activity easier to understand.

---

## 🎯 Business Problem

A coffee shop generates a large number of transactions across different products, categories, locations, dates, and times.

Looking at individual transactions does not provide an efficient way to understand overall business performance.

This project addresses that problem by organizing transaction data into meaningful analytical dimensions and presenting the results through an Excel dashboard.

The dashboard allows the analysis to answer questions such as:

- How much sales were generated?
- How many transactions occurred?
- Which products generated the highest sales?
- Which stores generated more sales and transactions?
- Which hours had the highest order quantity?
- Which categories contributed most to sales?
- How were transactions distributed by product size?
- Which weekdays recorded higher transaction activity?

---

## ❓ Business Questions

The analysis is designed to answer the following questions:

1. What are the overall sales and transaction volume?
2. What is the average bill per transaction?
3. What is the average quantity ordered per transaction?
4. Which hours have the highest order quantity?
5. Which product categories contribute the most to sales?
6. How are transactions distributed across product sizes?
7. Which store locations generate the highest sales?
8. Which store locations have the highest transaction volume?
9. Which product types generate the highest sales?
10. Which weekdays have the highest transaction activity?
11. How does the dashboard change when filtering by month?
12. How does the dashboard change when filtering by day?

---

# 📁 Dataset

## Raw Dataset

The raw workbook contains a single worksheet:

`Transactions`

### Dataset Summary

| Attribute | Details |
|---|---|
| Records | 149,116 |
| Columns | 11 |
| Period | January 1, 2023 – June 30, 2023 |
| Stores | 3 |
| Product Categories | 9 |
| Product Types | 29 |
| Product Details | 80 |
| Unique Transactions | 149,116 |

### Raw Data Columns

| Field | Description |
|---|---|
| `transaction_id` | Unique transaction identifier |
| `transaction_date` | Date of the transaction |
| `transaction_time` | Time of the transaction |
| `transaction_qty` | Quantity purchased |
| `store_id` | Store identifier |
| `store_location` | Store location |
| `product_id` | Product identifier |
| `unit_price` | Price per unit |
| `product_category` | Product category |
| `product_type` | Product type |
| `product_detail` | Detailed product description |

---

## 📘 Analysis Workbook

The analysis workbook contains three worksheets:

| Sheet | Purpose |
|---|---|
| `Coffee Shop Sales` | Prepared transaction-level dataset and analytical fields |
| `Dashboard` | Interactive dashboard |
| `Pivot Table` | Supporting PivotTable analysis |

The `Coffee Shop Sales` worksheet contains **18 columns**.

In addition to the original transaction fields, the analysis contains:

| Analytical Field | Purpose |
|---|---|
| `Size` | Product/order size classification |
| `Total_Bill` | Transaction-level bill amount |
| `Month Name` | Month-based filtering and analysis |
| `Day Name` | Day-based filtering and analysis |
| `Hour` | Hour-based analysis |
| `Day of Week` | Numeric weekday representation |
| `Month` | Numeric month representation |

---

# 🧹 Data Preparation

The analysis workbook contains prepared fields that extend the original transaction dataset for analytical use.

### Preparation performed

- Created `Total_Bill` from transaction quantity and unit price.
- Added product/order `Size` classification.
- Extracted `Hour` from transaction time.
- Created `Month Name`.
- Created `Month`.
- Created `Day Name`.
- Created `Day of Week`.
- Prepared fields for PivotTable aggregation.
- Prepared fields used by dashboard filters and charts.

### Data Validation

The provided raw dataset contains:

- **149,116 transaction records**
- No blank values across the 11 raw-data columns.
- No duplicate `transaction_id` values.
- No duplicate complete rows.

The analysis dataset also contains no blank values across its 18 fields.

---

# 📈 Analysis Performed

| Analysis | Purpose |
|---|---|
| **Sales Analysis** | Measure overall sales generated by transactions |
| **Footfall Analysis** | Measure transaction-based customer activity |
| **Hourly Analysis** | Understand order quantity throughout the day |
| **Category Analysis** | Compare sales contribution by product category |
| **Size Analysis** | Understand transaction distribution by size |
| **Product Analysis** | Identify highest-selling product types |
| **Store Analysis** | Compare sales and transaction activity by store |
| **Weekday Analysis** | Compare transaction activity across weekdays |
| **Month Analysis** | Explore dashboard results by selected month |
| **Day Analysis** | Explore dashboard results by selected weekday |

---

# 📌 Key Performance Indicators

The dashboard contains four primary KPI cards.

| KPI | Current Dashboard Value | Meaning |
|---|---:|---|
| **Total Sales** | **$698,812.33** | Total transaction sales |
| **Total Footfall** | **149,116** | Number of transactions |
| **Avg Bill/Person** | **$4.69** | Average sales value per transaction |
| **Avg Order/Person** | **1.4** | Average quantity ordered per transaction |

### KPI Definitions

**Total Sales**

Total value generated from all transaction bills.

**Total Footfall**

The dashboard uses transaction count as its footfall measure. Therefore, this metric represents **transaction-based activity**, not a separately measured unique-customer count.

**Average Bill/Person**

Calculated as total sales divided by the number of transactions.

**Average Order/Person**

Calculated as total quantity ordered divided by the number of transactions.

---

# 🖥️ Dashboard

The project includes an interactive Excel dashboard designed to provide a consolidated view of coffee shop performance.

## Dashboard Preview

![Coffee Shop Sales Analytics Dashboard](Coffee%20Sales%20%26%20Business%20Performance%20Dashboard.png)

### Dashboard Components

The dashboard contains:

| Component | Purpose |
|---|---|
| **Total Sales** | Displays overall sales |
| **Total Footfall** | Displays transaction volume |
| **Avg Bill/Person** | Displays average transaction value |
| **Avg Order/Person** | Displays average quantity per transaction |
| **Quantity Ordered Based on Hour** | Shows order quantity by hour |
| **Categories % Distribution Based on Sales** | Shows category contribution to sales |
| **% Size Distribution Based on Orders** | Shows transaction distribution by size |
| **Footfall and Sales Over Store Location** | Compares stores |
| **Top 5 Products Based on Sales** | Shows highest-selling product types |
| **Order On Weekday** | Compares weekday transaction activity |
| **Month Name Filter** | Filters dashboard by month |
| **Day Name Filter** | Filters dashboard by weekday |

---

# ✨ Dashboard Features

- ✓ Interactive Month Name filtering
- ✓ Interactive Day Name filtering
- ✓ KPI-based reporting
- ✓ Hourly order analysis
- ✓ Category sales distribution
- ✓ Product size distribution
- ✓ Store-level sales comparison
- ✓ Store-level transaction comparison
- ✓ Top 5 product analysis
- ✓ Weekday transaction analysis
- ✓ PivotTable-based reporting
- ✓ Excel dashboard visualization

---

# 🔎 Key Insights

The following observations are based on the provided transaction data.

## 1. Overall Sales Performance

The dataset generated:

### **$698,812.33**

in total sales across:

### **149,116 transactions**

The calculated average transaction value is approximately:

### **$4.69**

The average quantity ordered per transaction is approximately:

### **1.44 items**

---

## 2. Category Sales Contribution

The largest sales contributions come from **Coffee** and **Tea**.

| Product Category | Sales | Share of Total Sales |
|---|---:|---:|
| Coffee | $269,952.45 | 38.63% |
| Tea | $196,405.95 | 28.11% |
| Bakery | $82,315.64 | 11.78% |
| Drinking Chocolate | $72,416.00 | 10.36% |
| Coffee beans | $40,085.25 | 5.74% |
| Branded | $13,607.00 | 1.95% |
| Loose Tea | $11,213.60 | 1.61% |
| Flavours | $8,408.80 | 1.20% |
| Packaged Chocolate | $4,407.64 | 0.63% |

### Observation

Coffee and Tea together account for approximately:

**66.74% of total sales.**

---

## 3. Top 5 Product Types by Sales

| Product Type | Sales | Share of Total Sales |
|---|---:|---:|
| Barista Espresso | $91,406.20 | 13.08% |
| Brewed Chai tea | $77,081.95 | 11.03% |
| Hot chocolate | $72,416.00 | 10.36% |
| Gourmet brewed coffee | $70,034.60 | 10.02% |
| Brewed Black tea | $47,932.00 | 6.86% |

These five product types together contribute approximately:

**51.35% of total sales.**

---

## 4. Store Performance

The analysis covers three store locations.

| Store Location | Transactions | Sales |
|---|---:|---:|
| Hell's Kitchen | 50,735 | $236,511.17 |
| Astoria | 50,599 | $232,243.91 |
| Lower Manhattan | 47,782 | $230,057.25 |

### Observation

Hell's Kitchen has the highest transaction count and the highest total sales among the three locations in the dataset.

---

## 5. Hourly Order Quantity

The analysis shows significant differences in order quantity across operating hours.

| Hour | Quantity Ordered |
|---:|---:|
| 6 | 6,865 |
| 7 | 19,449 |
| 8 | 25,197 |
| 9 | 25,370 |
| **10** | **26,713** |
| 11 | 14,035 |
| 12 | 12,690 |
| 13 | 12,439 |
| 14 | 12,907 |
| 15 | 12,923 |
| 16 | 12,881 |
| 17 | 12,700 |
| 18 | 10,826 |
| 19 | 8,595 |
| 20 | 880 |

### Observation

The highest recorded order quantity occurs at:

**10:00 — 26,713 items**

The lowest recorded quantity occurs at:

**20:00 — 880 items**

---

## 6. Weekday Transaction Activity

| Day | Transactions |
|---|---:|
| Friday | 21,701 |
| Thursday | 21,654 |
| Monday | 21,643 |
| Wednesday | 21,310 |
| Tuesday | 21,202 |
| Sunday | 21,096 |
| Saturday | 20,510 |

### Observation

Friday records the highest transaction count, while Saturday records the lowest transaction count among the seven weekdays.

---

## 7. Order Size Distribution

The dashboard groups transactions into four size categories.

| Size | Transactions | Share |
|---|---:|---:|
| Regular | 45,789 | 30.71% |
| Large | 44,885 | 30.10% |
| Not Defined | 44,518 | 29.85% |
| Small | 13,924 | 9.34% |

### Observation

Regular and Large transactions together represent approximately:

**60.81% of recorded transactions.**

The relatively large **Not Defined** group is also a useful data-quality point for further investigation.

---

# 💡 Business Recommendations

The recommendations below are separated from the observations so that the analysis does not confuse an observed result with a proposed business action.

## Product Performance

**Observed from the data:**  
The five highest-selling product types are Barista Espresso, Brewed Chai tea, Hot chocolate, Gourmet brewed coffee, and Brewed Black tea.

**Potential business action:**  
These products can receive closer attention when reviewing inventory planning, product availability, and promotional opportunities.

---

## Store Performance

**Observed from the data:**  
Hell's Kitchen has the highest transaction count and sales among the three locations.

**Potential business action:**  
Store-level performance can be reviewed individually to understand differences in demand and sales contribution.

---

## Peak-Hour Planning

**Observed from the data:**  
10:00 records the highest order quantity, with 08:00 and 09:00 also showing high activity.

**Potential business action:**  
These periods can be considered when reviewing staffing, inventory availability, and service capacity.

---

## Weekday Planning

**Observed from the data:**  
Friday, Thursday, and Monday have the highest transaction counts.

**Potential business action:**  
Weekday transaction patterns can be considered when planning operational resources and demand coverage.

---

# 🛠️ Tools & Excel Techniques

## Primary Tool

### Microsoft Excel

The project uses Microsoft Excel for:

- Data preparation
- Data analysis
- Aggregation
- PivotTables
- PivotCharts
- Dashboard development
- Interactive filtering
- Business reporting

---

## Excel Techniques Used

### 📊 Excel Table

The transaction-level analysis data is organized into an Excel Table.

### 🔄 PivotTables

PivotTables are used to aggregate transaction information by dimensions such as:

- Hour
- Day
- Product Category
- Product Type
- Store Location
- Size

### 📈 PivotCharts / Charts

The dashboard visualizes the aggregated results using charts for:

- Hourly quantity
- Category contribution
- Size distribution
- Store performance
- Product sales
- Weekday activity

### 🎛️ Slicers / Filters

Interactive filtering is available for:

- Month Name
- Day Name

### 🧮 Calculated Analytical Fields

Additional fields were prepared for:

- Total Bill
- Size
- Month
- Month Name
- Day Name
- Day of Week
- Hour

---

# 🔄 Project Workflow

```mermaid
flowchart TD
    A[Raw Transaction Data] --> B[Data Preparation]
    B --> C[Analytical Fields]
    C --> D[PivotTable Analysis]
    D --> E[KPI Calculation]
    D --> F[Data Visualization]
    E --> G[Interactive Excel Dashboard]
    F --> G
    G --> H[Business Insights]
    H --> I[Potential Business Actions]
