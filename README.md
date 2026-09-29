# Port Logistics Turnaround Optimization & AI-Readiness Assessment

## 🚢 Overview
This repository contains an end-to-end data analytics business case applied to maritime port operations. The primary objective is to analyze Terminal Operating System (TOS) gate and yard logs to identify the root causes of high truck turnaround times, and to establish the clean data infrastructure required for future Artificial Intelligence (AI) deployment.

This project is a practical application of the **Portuaria IA Framework (Plan · Deliver · Grow)**, bridging core **Data Literacy** with **Applied Business AI** strategy.

## 🎯 Business Problem (PLAN)
**Context:** The terminal experiences severe yard congestion during peak hours, leading to breached Service Level Agreements (SLAs) with trucking companies. The target SLA for truck turnaround time is 45 minutes.

**The Dual Task:**
1. **Immediate Analytics Goal:** Identify operational bottlenecks causing turnaround delays.
2. **AI Consultancy Goal:** Assess data quality and propose a roadmap for predictive Machine Learning models for dynamic yard resource allocation.

## 🛠️ Data Processing & Engineering (DELIVER)
Clean data is the critical foundation for any AI model. 
* **Data Source:** A synthesized dataset of 1,000 records mirroring real-world NAVIS N4 / CAMCO TOS exports.
* **Tools:** Python (Pandas, NumPy, Matplotlib, Seaborn) and SQL.
* **Process:** Cleaned operational logs, calculated exact turnaround times, and engineered new features (e.g., `hour_of_day`) to identify congestion patterns.

*You can view the full interactive Python Notebook and visualizations on my Kaggle:*
👉 **[View Interactive Notebook on Kaggle](https://www.kaggle.com/code/lilimedina/port-logistics-turnaround)**

## 📊 Exploratory Data Analysis & Insights (DELIVER)
Based on the analysis, two critical operational insights emerged:
* **Insight 1: Peak Hour Congestion Breaches SLAs.** Average turnaround times drastically exceed the 45-minute SLA target during the 12:00 shift handover and the afternoon peak (14:00 - 15:00).
* **Insight 2: Automated vs. Manual Gate Efficiency.** Automated (CAMCO) gates process trucks significantly faster and with lower variance compared to Manual gates.

## 🚀 Strategic Recommendations & AI Business Case (GROW)
Translating data literacy into business impact, the following roadmap is proposed:

### Phase 1: Short-Term Operational Fixes
* **Dynamic Quotas:** Implement dynamic gate appointment quotas based on historical congestion heatmaps to flatten the arrival curve.
* **Shift Handover Mitigation:** Restructure the 12:00 shift handovers to maintain a skeleton crew.

### Phase 2: The AI Business Case
* **The AI Opportunity:** The data pipeline established here is clean, structured, and ready to train a predictive Machine Learning model.
* **Proposed AI Solution:** Develop an AI-driven dynamic yard allocation system to predict peak truck arrivals and automatically pre-position Rubber Tyred Gantry (RTG) cranes in congested yard blocks.

## 💻 Repository Structure
* `notebook_camco.ipynb`: The main Jupyter Notebook containing the data generation, processing, and visualization code.
* `port_logistics_data.csv`: The simulated TOS dataset generated for this analysis.
* `README.md`: Project documentation and executive summary.

---
*This project was developed by Liliana Medina as part of the Google Data Analytics Professional Certificate and the Portuaria IA framework.*
