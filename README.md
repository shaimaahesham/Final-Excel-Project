# Adventure Works 2012 - Data Analysis & Dashboard

[Final_Analysis_Dashboard.png]


## 📋 Project Overview

A comprehensive data analysis project on Adventure Works 2012 dataset using Excel, focusing on **data modeling and power querying** rather than visual aesthetics. This project demonstrates the importance of proper data architecture and preprocessing in analytics.

**Key Philosophy:** 80% of the work is data prep and modeling. Once your data is clean and properly structured, the insights build themselves.

---

## 🏗️ Data Architecture

### Star Schema Design

The project implements a classic **star schema** with a central fact table surrounded by dimension tables:

#### **Fact Table:**
- **Fact_Orders** - Central fact table containing:
  - SalesOrderID
  - CustomerID
  - ProductID
  - TerritoryID
  - ShipMethodID
  - OrderQty, UnitPrice, LineTotal
  - SubTotal, TaxAmt, Freight, TotalDue
  - Date_Key (for temporal relationships)

#### **Dimension Tables:**
- **Dim_Date** - Temporal dimension
  - OrderDate, Year, Month Name, Day, Quarter
  - Date_key (primary key)
  
- **Dim_Products** - Product dimension
  - ProductID, Product, Category
  - SubCategory, Color
  
- **Dim_Territories** - Geographic dimension
  - TerritoryID, Territory
  
- **Dim_ShipMethod** - Shipping dimension
  - ShipMethodID, ShipMethod

---

## 📊 Analysis Components

### Key Metrics (KPIs)
- **Total Sales:** $2,926,870,124
- **Number of Orders:** 31,465
- **Number of Customers:** 19,119
- **Total Quantity Sold:** 274,914
- **Subtotal:** $2,596,470,457
- **Total Tax:** $251,809,269
- **Total Freight:** $78,690,398

### Analysis Dimensions
1. **Sales Performance**
   - Total Sales per Month
   - Sales by Territory
   - Sales by Category
   - Top 5 Products by Sales

2. **Order Analysis**
   - Number of Orders per Category
   - Orders by Color
   - Customer Distribution by Territory

3. **Product Insights**
   - Quantity by Categories (Bikes: 40%, Clothing: 29%, Components: 18%, Accessories: 13%)
   - Sales Performance by Product Category

4. **Geographic Analysis**
   - Customer base across 10 territories
   - Sales distribution by territory
   - Territory-wise performance metrics

---

## 🛠️ Tools & Technologies

- **Excel 2016+** (Power Query, Pivot Tables)
- **Power Query** - Data transformation and cleaning
- **Pivot Tables** - Aggregation and summarization
- **Data Model** - Relational schema design

---

## 📁 Project Files

```
Adventure_Works_Analysis/
├── Final_Analysis_Dashboard.png    # Interactive dashboard with KPIs and visualizations
├── Final_Data_Model.png            # Star schema diagram
├── Pivot_Tables.png                # Summary tables and analysis
└── README.md                       # This file
```

---

## 🔄 Data Processing Workflow

### 1. **Data Extraction**
   - Raw Adventure Works 2012 data imported into Excel

### 2. **Power Query Transformation**
   - Data cleaning and validation
   - Column renaming and formatting
   - Removing duplicates and handling missing values
   - Creating calculated columns

### 3. **Data Modeling**
   - Establishing relationships between tables
   - Creating the star schema
   - Setting up primary and foreign keys
   - Optimizing table structure for analysis

### 4. **Analysis Layer**
   - Building pivot tables for different dimensions
   - Creating KPI cards
   - Developing interactive dashboard
   - Generating insights through cross-tabulation

---

## 📈 Key Insights

- **Best Performing Month:** September (~$306.89M in sales)
- **Top Territory:** United Kingdom ($571.47M)
- **Most Popular Product:** AWC Logo Cap (highest sales)
- **Product Mix:** Bikes dominate sales at 40% of total quantity
- **Customer Base:** Concentrated in Australia (3,020 customers) and United Kingdom (3,335 customers)

---

## 💡 Data Quality & Preprocessing

- ✅ Handled missing values in dimensional attributes
- ✅ Standardized date formats across all temporal data
- ✅ Validated referential integrity between fact and dimension tables
- ✅ Created surrogate keys for efficient relationships
- ✅ Optimized table relationships for query performance

---

## 🎯 Learning Outcomes

This project emphasizes:
1. **Data Modeling** - Star schema design principles
2. **Power Query** - ETL processes in Excel
3. **Relational Database Design** - Dimensional modeling
4. **Data Preprocessing** - The critical foundation of analytics
5. **Dashboard Development** - Converting processed data into actionable insights

---

## 📌 How to Use This Project

1. **Review the Data Model** (`Final_Data_Model.png`)
   - Understand the dimensional structure
   - Review table relationships

2. **Explore the Dashboard** (`Final_Analysis_Dashboard.png`)
   - Filter by date range, ship method, color, and product category
   - Analyze multi-dimensional views

3. **Study the Pivot Tables** (`Pivot_Tables.png`)
   - See aggregation logic
   - Understand calculation methods

4. **Learn from the Process**
   - Focus on data architecture, not visual design
   - Prioritize data quality and relationships
   - Let clean data speak for itself

---

## 🚀 Future Enhancements

- Integration with Power BI for advanced visualizations
- Predictive modeling for sales forecasting
- Customer segmentation analysis
- Time-series forecasting
- Cohort analysis

---

## 📝 Notes

- The emphasis of this project is on **data architecture and preprocessing**
- Power Query transformation was prioritized over dashboard aesthetics
- All analysis is based on properly normalized and validated data
- The star schema ensures scalability and maintainability

---

## 👤 Author Notes

This analysis demonstrates that effective data analytics is 80% data preparation and modeling, and 20% visualization. The real value lies in having clean, well-structured data with proper relationships—not in fancy dashboard aesthetics.

---

**Last Updated:** April 2026  
**Data Source:** Adventure Works 2012 Dataset  
**Analysis Type:** Exploratory Data Analysis (EDA) with Star Schema Design
