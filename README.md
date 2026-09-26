# Tanishq-Style Jewelry Retail Analytics Suite

### End-to-End Excel Data Model & Executive Dashboard

> **Portfolio Project | Retail Analytics | Excel | Business Intelligence | Data Modeling**

---

## 📌 Project Overview

This project is an end-to-end **retail analytics solution for a multi-store Indian jewelry business**, modeled around a Tanishq-style retail environment.

The workbook analyzes sales, inventory, procurement, stores, customers, employees, finance, and omnichannel performance using a **60-sheet Excel analytical model** built around a structured **Fact + Dimension (star-schema) architecture**.

The objective was to transform raw transactional data into **management-ready KPIs, business insights, operational analysis, and executive dashboards**.

**Important:** The dataset is synthetic and was generated using Python for portfolio/learning purposes.

---

## 🎯 Business Scenario

The simulated organization operates:

* 20 retail stores across India
* Physical stores + online/app channel
* Gold, Diamond, Platinum, Silver, and Studded jewelry
* Multiple product categories and price bands
* Store, inventory, procurement, finance, HR, and CRM operations

The project was designed to answer real-world business questions that a **MIS Executive, Business Analyst, Data Analyst, or Operations Analyst** may encounter.

---

# 📊 Dataset Overview

| Component          |             Details |
| ------------------ | ------------------: |
| Sales Transactions |              87,254 |
| Inventory Records  |              54,000 |
| Purchase Orders    |              31,074 |
| Customers          |               5,000 |
| Online Orders      |               7,000 |
| Stores             |                  20 |
| SKUs               |                 150 |
| Analysis Period    | Jan 2025 – Jun 2026 |
| Excel Sheets       |                  60 |
| Business Modules   |                   9 |

---

# 🗂️ Core Data Tables

## Fact_Sales

Main transactional sales table containing:

* Transaction ID
* Date
* Store ID
* SKU
* Customer ID
* Staff ID
* Quantity
* Weight (grams)
* Gold Rate / gram
* Making Charge Value
* Stone Value
* Old Gold Exchange Value
* Gross Value
* Discount %
* Discount Value
* Net Value
* Payment Mode

## Supporting Tables

### Inventory

* Opening Stock
* Received Stock
* Sold Stock
* Closing Stock
* Store
* SKU
* Month

### Purchase Orders

* PO ID
* Vendor
* SKU
* Quantity
* Order Date
* Lead Time
* Replenishment Event

### Customers

* Customer ID
* Recency
* Frequency
* Monetary Value
* RFM Segment

### Staff

* Staff ID
* Role
* Store
* Tenure
* Performance-related attributes

### Online Sales

* Online Order ID
* Customer
* SKU
* Channel
* Delivery Mode
* Order Value

### Returns

* Return Reason
* RTV Flag
* Product
* Store
* Transaction information

---

# 🏪 Store Network

The model contains **20 stores across India**, representing:

* Metro cities
* Tier-1 cities
* Tier-2 cities

Store formats include:

* Flagship
* Standard
* Compact

---

# 💎 Product Portfolio

The model contains **150 SKUs** across:

### Metals / Categories

* Gold
* Diamond
* Platinum
* Silver
* Studded

### Product Types

* Necklaces
* Rings
* Earrings
* Bangles
* Bracelets
* Pendants
* Chains
* Mangalsutras

---

# 📅 Analysis Period

**January 2025 – June 2026**

Total analysis period:

**18 months**

---

# 🔎 Analysis Performed

## 1. Sales Analytics

* Sales trend analysis
* Category performance
* Collection performance
* Product velocity
* Fast-moving products
* Slow-moving products
* Dead movers
* Price-band analysis
* Target vs Achievement
* Seasonal sales analysis
* Festival performance
* Promotional campaign analysis

---

## 2. Inventory Analytics

* Inventory ageing
* Stock turnover
* Sell-through %
* ABC classification
* XYZ classification
* Stock-out risk
* Safety stock
* Reorder point
* EOQ
* Inventory efficiency
* Non-moving inventory

---

## 3. Merchandising Analytics

* Category performance
* SKU velocity
* Price-band performance
* Product profitability
* Collection analysis
* Discount analysis
* Gross margin analysis
* Making-charge realization

---

## 4. Supply Chain Analytics

* Purchase order analysis
* Vendor performance
* Lead-time analysis
* Replenishment analysis
* EOQ optimization
* Purchase frequency
* Ordering-cost analysis
* Stock transfer analysis
* On-time delivery analysis

---

## 5. Store Performance Analytics

* Store revenue
* Store profitability
* Sales per square foot
* GMROI
* Store target achievement
* Inventory efficiency
* Category contribution
* Store-level performance comparison

---

## 6. Commercial Analytics

* Discount analysis
* Gross margin
* Making-charge realization
* Promotional campaign ROI
* Price-band performance
* Revenue contribution

---

## 7. Finance Analytics

Built a simplified business-level financial model covering:

**Revenue → Gross Profit → Operating Expenses → EBITDA**

Analysis includes:

* Revenue
* Gross Margin
* Operating Expenses
* EBITDA
* EBITDA Margin
* Working Capital
* Cash Conversion Cycle

---

## 8. HR Analytics

* Employee analysis
* Staff roles
* Tenure
* Attrition
* Incentive payout
* Payroll structure
* Store-level workforce analysis

---

## 9. CRM Analytics

Used **RFM analysis** to segment customers based on:

* Recency
* Frequency
* Monetary Value

Customer segments include behavioral groups such as:

* Champions
* Loyal Customers
* Potential Loyalists
* At Risk
* Lost Customers

---

## 10. Omnichannel Analytics

Compared:

**Online vs In-Store**

Analysis includes:

* Revenue
* Category performance
* Product affinity
* Customer behavior
* Delivery mode
* Channel contribution

---

# 📈 Key KPIs

The project calculates and tracks:

* Revenue
* Gross Margin %
* EBITDA Margin
* GMROI
* Inventory Turnover
* Sell-Through %
* Forecast Accuracy
* MAPE
* EOQ Potential Savings
* Attrition Rate
* RFM Segment Distribution
* On-Time Delivery %
* Cash Conversion Cycle
* Ageing Stock %
* Target Achievement %
* Sales per Sq. Ft.

---

# 🧮 Excel Techniques Used

The analytical workbook was built using native Excel formulas.

### Main Functions

* `SUMIFS`
* `COUNTIFS`
* `AVERAGEIFS`
* `INDEX`
* `MATCH`
* `IF`
* `IFERROR`
* `SUMPRODUCT`
* `RANK`
* `LARGE`
* `SMALL`
* `PERCENTILE`

### Excel Features

* Excel Tables
* Structured References
* Conditional Formatting
* RAG Status Indicators
* Color Scales
* Data Validation
* Dropdown Controls
* Cross-Sheet Formula Architecture
* Dynamic Assumption Cells
* What-If Analysis

---

# 🧹 Data Quality & Validation

A dedicated **Data Quality Validation** module contains **17 automated validation checks**.

Checks include:

* Orphaned foreign keys
* Missing values
* Negative values
* Invalid dates
* Out-of-range values
* Purchase order anomalies
* Inventory inconsistencies
* Referential integrity

### Data Integrity Issues Identified

During development, several data integrity problems were identified and corrected.

### Inventory Issue

Approximately **24% of recorded sales volume** initially showed more stock sold than stock received.

The issue was traced to incorrect safety-cap logic and corrected across the **54,000 inventory records**.

### Purchase Order Issue

The initial purchase-order dataset represented only approximately **10% of the intended replenishment volume**.

The dataset was subsequently rebuilt into **31,074 replenishment events**.

### Margin Calculation Issue

A margin calculation was producing the correct numerical result through indirect algebra.

It was rewritten as a direct and auditable:

**Revenue − Cost = Gross Profit**

approach.

---

# 📊 Dashboard Structure

The workbook contains approximately **60 sheets** organized into 9 business modules.

### Business Modules

1. Merchandising
2. Inventory
3. Supply Chain
4. Store Performance
5. Commercial
6. Finance
7. HR
8. CRM
9. Compliance

---

# 📑 Executive Reporting

The workbook includes three levels of management reporting:

### Daily Business Review

Operational monitoring and immediate exceptions.

### Weekly Business Review

Performance trends, operational issues, and business drivers.

### Monthly Business Review

Management-level performance, profitability, inventory, finance, and strategic KPIs.

---

# 🚦 Executive RAG Scorecard

A board-level KPI scorecard was created using:

* 🟢 Green — Within target
* 🟡 Amber — Requires attention
* 🔴 Red — Requires management action

The scorecard consolidates major business KPIs into a single executive view.

---

# 🔬 Forecasting & Inventory Optimization

The project includes:

### Demand Forecasting

Forecast accuracy is evaluated using:

**MAPE — Mean Absolute Percentage Error**

### EOQ

Economic Order Quantity was used to analyze optimal purchasing quantities.

### Safety Stock

Safety-stock assumptions can be changed through editable input cells.

### Reorder Point

Reorder calculations incorporate demand and lead-time assumptions.

---

# 🎛️ What-If Scenario Simulator

A scenario simulator allows management to change assumptions such as:

* Discount %
* Gold Rate
* Ordering Cost
* Service-Level Z-Score
* Discount Elasticity

Changes propagate through dependent calculations to evaluate potential impact on:

* Revenue
* Margin
* Inventory
* Profitability

The model is **dynamic and formula-driven**, rather than VBA/macro automated.

---

# 💡 Key Business Insights

## 1. Revenue vs Profitability

Gross margins appeared healthy at approximately **15–17%**.

However, after incorporating rent, staff costs, and other operating expenses, the modeled **EBITDA margin was approximately 1.46%**.

This demonstrates why revenue and gross margin alone are insufficient for evaluating overall business performance.

---

## 2. Stock Transfers

Approximately **45% of historical stock transfers** were classified as questionable based on the project's transfer-need criteria.

This highlighted an opportunity to improve stock-transfer approval rules.

---

## 3. Festival Performance

**Dhanteras** generated the strongest modeled sales uplift among the analyzed festivals:

**+261% vs baseline**

---

## 4. Diamond Procurement

EOQ analysis for the Diamond category indicated potential annual ordering-cost savings of approximately:

**₹5–17 lakh**

depending on the assumptions used.

---

## 5. Channel Affinity

The analysis identified a category-channel pattern:

* **Studded jewelry → stronger online sales**
* **Gold jewelry → stronger in-store sales**

This suggests different merchandising and channel strategies may be appropriate for different product categories.

---

# 🎯 Business Questions Answered

The project was designed to answer questions such as:

### Sales

* Which stores generate the highest revenue?
* Which categories contribute the most sales?
* Which price bands perform best?
* Which products are fast-moving?

### Inventory

* Which products are ageing?
* Which SKUs are at stock-out risk?
* Which products should be reordered?
* Which products are tying up inventory?

### Procurement

* Are purchase orders being placed efficiently?
* Which vendors have better performance?
* Can ordering frequency be optimized?
* How much could EOQ reduce ordering costs?

### Stores

* Which stores are generating profitable sales?
* Which stores have poor inventory productivity?
* Which stores are achieving their targets?

### Customers

* Who are the highest-value customers?
* Which customers are Champions?
* Which customers are at risk?
* Are loyalty classifications aligned with actual customer behavior?

### Finance

* What is the true bottom-line profitability?
* How does EBITDA differ from gross margin?
* What is the working-capital impact?

---

# 🏗️ Data Model Architecture

The workbook follows a **star-schema-inspired architecture**.

### Fact Tables

* Fact_Sales
* Fact_Inventory
* Fact_PurchaseOrders
* Fact_OnlineSales
* Fact_Returns

### Dimension Tables

* Dim_Date
* Dim_Store
* Dim_Product
* Dim_Customer
* Dim_Staff
* Dim_Vendor
* Dim_Channel

This structure makes the analytical model easier to extend to:

* SQL
* Power BI
* Other BI platforms

---

# 🐍 Python Usage

Python was used **only for synthetic dataset generation**.

Python generated realistic-looking:

* Sales transactions
* Inventory records
* Customer data
* Purchase orders
* Online orders
* Supporting dimensions

The analytical calculations were then performed in **Excel**.

### Important

The Excel workbook itself is **100% Excel-based for analytical calculations**.

Python was not used as the analytical engine inside the workbook.

---

# 🚫 Tools Not Used

For transparency, this project does **not** claim the use of:

* Power Query
* Power Pivot
* PivotTables
* VBA

The project intentionally demonstrates what can be built using **native Excel formulas and structured data modeling**.

---

# ⚙️ Automation Approach

There is no VBA or macro-based automation.

Instead, the workbook uses:

* Formula-driven calculations
* Editable assumption cells
* Structured references
* Cross-sheet dependencies
* Dynamic KPI calculations
* Conditional formatting
* Data validation

Therefore, the workbook is **dynamic and self-updating**, rather than macro-automated.

---

# 📁 Suggested GitHub Repository Structure

```text
Tanishq-Jewelry-Retail-Analytics/
│
├── README.md
│
├── Excel/
│   └── Jewelry_Retail_Analytics.xlsx
│
├── Documentation/
│   ├── Data_Dictionary.xlsx
│   ├── Business_Requirements.md
│   └── Methodology.md
│
├── Screenshots/
│   ├── Executive_Dashboard.png
│   ├── Sales_Dashboard.png
│   ├── Inventory_Dashboard.png
│   ├── Supply_Chain_Dashboard.png
│   ├── Finance_Dashboard.png
│   ├── CRM_Dashboard.png
│   └── Data_Quality.png
│
└── Data/
    └── README.md
```

> **Note:** Do not upload sensitive real company data. The dataset used in this project is synthetic.

---

# 🛠️ Technology Stack

| Technology      | Purpose                                          |
| --------------- | ------------------------------------------------ |
| Microsoft Excel | Data modeling, calculations & dashboards         |
| Excel Formulas  | Analytical calculations                          |
| Python          | Synthetic dataset generation                     |
| GitHub          | Project version control & portfolio presentation |

---

# 📚 Skills Demonstrated

### Data Analytics

* Data Cleaning
* Data Validation
* Exploratory Data Analysis
* KPI Development
* Business Analysis
* Trend Analysis
* Segmentation
* Forecast Accuracy
* Scenario Analysis

### Excel

* Advanced Formula Development
* Data Modeling
* Excel Tables
* Structured References
* Conditional Formatting
* Data Validation
* Dashboard Development
* What-If Analysis

### Business

* Retail Analytics
* Inventory Management
* Supply Chain
* Procurement
* Store Operations
* Financial Analysis
* CRM Analytics
* HR Analytics
* Omnichannel Analytics

---

# 🚀 Future Enhancements

Potential future versions of this project can extend the model into:

* Power BI dashboards
* SQL database implementation
* Python-based analytics
* Automated ETL pipelines
* Advanced demand forecasting
* Machine-learning-based customer segmentation
* Automated reporting
* Cloud database integration

---

# ⚠️ Project Disclaimer

This is a **portfolio and learning project**.

The company, stores, customers, employees, transactions, financial figures, vendors, and other business data are **synthetically generated** and do not represent actual Tanishq/Titan company data.

The business scenario is inspired by a large Indian jewelry-retail environment for educational and analytical modeling purposes.

---

# 👤 Author

**Rajdeep Kumar**

### Focus Areas

* MIS & Business Analytics
* Excel Analytics
* Operations Analytics
* Supply Chain Analytics
* Data Visualization
* Business Intelligence

---

## ⭐ Project Objective

The primary objective of this project was to demonstrate the ability to take a large, structured business dataset and build an **end-to-end analytical solution in Excel** — from data validation and modeling through KPI calculation, business analysis, scenario modeling, and executive reporting.

**The project focuses on solving business problems, not simply creating Excel dashboards.**
