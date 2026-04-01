# 📊 E-Commerce Profitability & RTO Risk Analytics Engine

## 🎯 Objective
Built an analytics system to measure **true campaign profitability (Net ROI)** by including:
- Return-to-Origin (RTO) losses  
- Attribution gaps between ad platforms and analytics tools  

This helps answer:
> Are we actually making money from our campaigns?

---

## 🚨 Business Problem
- **Attribution Issue:** Ad platforms over-report revenue, leading to wrong decisions  
- **RTO Losses:** High COD orders result in failed deliveries and revenue loss  
- **Limited Visibility:** Hard to connect campaigns, customers, and logistics losses  

---

## 🏗️ Dataset
- Created a **synthetic dataset using Gemini**, based on 4 years of performance marketing experience  
- Designed to reflect real-world challenges:
  - Differences between platform and GA4 data  
  - Higher RTO in COD orders  
  - Multi-channel campaign data  

- Built using a **star schema** for better analysis  

---

## ⚙️ Data Architecture
- Data stored and queried in **Google BigQuery**  
- Data transformed using **SQL (joins, CTEs, window functions)**  
- Connected to **Power BI** for modeling and dashboards  

**Flow:** BigQuery → Power BI  

---

## 🔍 Key Analysis

### 1. Profitability Analysis
- Calculated **Net ROI after RTO losses**  
- Found campaigns that looked profitable on ROAS but were actually loss-making  

### 2. Attribution Analysis
- Compared **platform vs GA4 revenue**  
- Identified gaps to avoid over-scaling campaigns  

### 3. RTO Analysis
- Identified high-risk:
  - Customers  
  - Products  
  - Locations  
- Found COD as a major reason for delivery failures  

### 4. Customer Segmentation
- Grouped customers based on risk level  
- Suggested actions:
  - High risk → avoid targeting  
  - Low risk → encourage prepaid  


## 🛠️ Tech Stack
- **SQL (BigQuery)**  
- **Power BI (DAX)**  
- Data sources modeled: GA4, Shopify, Meta Ads, Google Ads  

---

## 📈 Key Takeaway
> Platform ROAS can be misleading.  
> **Net ROI after RTO shows the real performance.**

---

## 🔗 Live Dashboard
https://app.powerbi.com/view?r=eyJrIjoiYjJhZTZlYmItZjMwNy00NjJiLTgwZDctY2U4YWVjNzZjZjI5IiwidCI6ImI4OTZkMGRjLWFjYjItNDI2OC1iNjVlLWRkZWMyMDdiNmZkZSJ9












