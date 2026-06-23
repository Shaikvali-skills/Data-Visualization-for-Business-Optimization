# Insigh BI - Data Visualization for Business Optimization

An end-to-end Business Intelligence solution built in Power BI to analyze the critical intersection between supply chain fulfillment and financial performance. 

## 🔗 Live Dashboard
[View Interactive Power BI Dashboard](https://app.powerbi.com/groups/bb85a59b-a6df-4224-a3b6-8fcdc068c30a/reports/10c4da01-e92a-44ad-9dac-ebf8f7e3a1b5/3b2ae56fd2901e800313?experience=power-bi)

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
As visualized in `Screenshot 2026-06-23 155039.png`, this view focuses on supply chain constraints:
* **Average Demand per Day:** 48.65 units
* **Average Availability per Day:** 24.70 units
* **Total Supply Shortage:** 61K units

### Page 2: Financial Performance & Impact Analysis
As visualized in `Screenshot 2026-06-23 155053.png`, this view tracks the financial damage driven by fulfillment gaps:
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
The data model blends operational tracking metrics with financial accounting fields. The primary tables utilized from the database and internal datasets include (refer to `image_175127.jpg` for the full fields list):
* **Demand/Availability Data:** `Availability`, `Demand`, `Order_Date_DD_MM_YYYY`, `Product_ID`, `Product_Name`, `Unit_Price`
* **MySQL Database Mirror:** Replicated transactional backend storing primary supply metrics.

---

## 🚀 How to Run this Project Locally
1. Clone this repository to your local machine.
2. Set up the local **MySQL Database** using the provided `.sql` schema script (if applicable).
3. Open the `Insigh_BI_Dashboard.pbix` file in Power BI Desktop.
4. Update the data source credentials to point to your MySQL instance.
5. Click **Refresh** to populate the data.
