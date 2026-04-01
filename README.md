# E-Commerce Profitability & RTO Risk Analytics Engine

### 🎯 The Objective
This project operates at the intersection of **Data Engineering**, **Business Strategy**, and **Marketing Analytics**. 

In e-commerce, front-end marketing metrics (like Platform ROAS) often paint an overly optimistic picture of profitability by ignoring back-end logistics. This analytics engine bridges that gap, calculating true **Net ROI** after accounting for Return-to-Origin (RTO) losses and multi-touch attribution discrepancies.

---

### 🚨 The Business Problem
1. **The Attribution Illusion:** Ad platforms inherently over-claim revenue. Relying solely on platform ROAS leads to scaling campaigns that are actually losing money.
2. **The RTO Bleed:** A high volume of Cash-on-Delivery (COD) orders results in delivery failures (RTOs), wiping out the profit margins of seemingly successful marketing campaigns. 
3. **Operational Silos:** Marketing teams rarely have a streamlined way to retroactively identify which specific customers or campaigns are driving the highest logistical losses.

---

### 🏗️ Data Engineering & Synthetic Generation
Instead of relying on clean, pre-packaged datasets, I engineered a custom synthetic dataset designed to mirror the actual complexities of a scaling e-commerce business. Drawing on four years of deep performance marketing experience, I modeled realistic data anomalies, including:
* Multi-touch attribution gaps between web analytics and ad platforms.
* Varying RTO probabilities based on payment methods (COD vs. Prepaid).
* Cross-channel spend discrepancies and dynamic customer risk profiles. 

This robust dataset allowed for the creation of a realistic Star Schema capable of stress-testing advanced DAX logic and complex SQL transformations.

---

### 🔍 Core Analytical Pillars

#### 1. Data Architecture 
* **Data Integration:** Unified fragmented data sources (backend order data, web analytics, and ad platform spend) using **Google BigQuery** and **SQL** (CTEs, Window Functions, Joins).
* **Relational Modeling:** Built a highly scalable **Star Schema**, utilizing conformed dimensions (`Dim_Date`, `Dim_Campaigns`, `Dim_Products`) to ensure perfect referential integrity across disparate fact tables.
* **Advanced DAX:** Engineered custom measures and context transitions to evaluate lifetime order histories and generate dynamic summaries.

#### 2. Commercial Strategy 
* **Revenue Degradation Tracking:** Visualized the exact pipeline from Gross Sales → Attributed Sales → Net Delivered Revenue, allowing executives to see the true cost of customer acquisition.
* **Process Optimization:** Translated raw logistical data into actionable exclusion lists. The Risk Segmentation matrix prescribes operational directives (e.g., "Remove from TG" or "Force Prepaid Only") to mitigate financial risk.
* **Simulated Business Impact:** Provided the data foundation required to identify high-risk segments and recover significant operating margin.

#### 3. Performance Tracking 
* **Attribution Reconciliation:** Identified and quantified attribution gaps between external analytics and ad platform reporting, stopping the over-scaling of unprofitable campaigns.
* **Spend Efficiency:** Highlighted high-spend, low-performing campaigns, shifting the optimization focus from "Cost Per Click" to "Cost Per Delivered Order."

---

### 🛠️ Tech Stack
* **BI & Visualization:** Power BI, DAX, Power Query
* **Data Storage & Manipulation:** Google BigQuery, SQL
* **Data Sources Modeled:** E-commerce Backend (Shopify), Web Analytics (GA4), Ad Platforms (Meta, Google)

📷 Get Interactive Report :
https://app.powerbi.com/view?r=eyJrIjoiYjJhZTZlYmItZjMwNy00NjJiLTgwZDctY2U4YWVjNzZjZjI5IiwidCI6ImI4OTZkMGRjLWFjYjItNDI2OC1iNjVlLWRkZWMyMDdiNmZkZSJ9










