# Insigh BI - Data Visualization for Business Optimization

An end-to-end Business Intelligence solution built in Power BI to analyze the critical intersection between supply chain fulfillment and financial performance. 

## 🔗 Live Dashboard
[View Interactive Power BI Dashboard](Insert_Your_Power_BI_Publish_Link_Here)

---

## 📌 Project Overview
The **Insigh BI** dashboard was engineered to solve a common enterprise problem: visibility gaps between sales demand, inventory availability, and bottom-line losses. By combining transactional data with operational logs, this dashboard exposes how severe supply shortages directly drive revenue leakage.

### Key Capabilities:
* **Fulfillment Mapping:** Tracks daily supply vs. demand metrics to spotlight inventory health.
* **Financial Leakage Auditing:** Quantifies total losses and calculates daily run-rate leakages to help management prioritize operational fixes.
* **Cross-Source Modeling:** Combines relational database management system schemas with transactional flat files.

---

## 📊 Dashboard Architecture & Metrics

### Page 1: Operational Efficiency & Supply Metrics
This view focuses on supply chain constraints:

![Operational Efficiency Dashboard](Screenshot%202026-06-23%20155039.png)

* **Average Demand per Day:** 48.65 units
* **Average Availability per Day:** 24.70 units
* **Total Supply Shortage:** 61K units

### Page 2: Financial Performance & Impact Analysis
This view tracks the financial damage driven by fulfillment gaps:

![Financial Performance Dashboard](Screenshot%202026-06-23%20155053.png)

* **Total Profit:** 301K
* **Total Loss:** 8M
* **Average Daily Loss:** 2.97K

---

## 🛠️ Tech Stack & Tools
* **BI Platform:** Power BI Desktop
* **Database:** MySQL Database (Relational storage for product tracking and inventory orders)
* **Data Prep:** Power Query (ETL processing, data cleaning, date formatting)
* **Modeling:** DAX (Data Analysis Expressions) for custom time-intelligence and aggregation metrics

---

## 🗄️ Data Model & Schema
The data model blends operational tracking metrics with financial accounting fields. The primary tables utilized from the database and internal datasets include:
* **Demand/Availability Data:** `Availability`, `Demand`, `Order_Date_DD_MM_YYYY`, `Product_ID`, `Product_Name`, `Unit_Price`
* **MySQL Database Mirror:** Replicated transactional backend storing primary supply metrics.

---

## 🚀 How to Run this Project Locally
1. Clone this repository to your local machine.
2. Set up the local **MySQL Database** using the provided `.sql` schema script (if applicable).
3. Open the `Insigh_BI_Dashboard.pbix` file in Power BI Desktop.
4. Update the data source credentials to point to your MySQL instance.
5. Click **Refresh** to populate the data.
