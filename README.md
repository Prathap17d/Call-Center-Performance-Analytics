# End-to-End Call Center Performance Analytics

## 📋 Project Overview
This project demonstrates an end-to-end data analytics workflow, taking raw operational call center data, engineering a clean data pipeline using **Python**, and designing an executive-level, interactive **Power BI** dashboard. The final multi-page application uncovers critical performance bottlenecks, maps SLA compliance across communication channels, and delivers actionable strategic recommendations to improve customer satisfaction (CSAT).

---

## 🛠️ Tech Stack & Tools Used
* **Data Cleaning & EDA:** Python 3 (Pandas, Jupyter Notebook)
* **Visualization & Analytics Engine:** Power BI Desktop
* **Calculations:** Data Analysis Expressions (DAX)
* **Design Frame:** Custom application-style UI layout with vector navigation icons

---

## 📊 Business Case Study (STAR Method)

### 🔹 Situation
An enterprise customer support network tracking over 32,000 monthly interactions noticed systemic drops in regional customer satisfaction. Executive leadership required deep visibility into operational metrics to identify underlying service friction points and reverse declining customer sentiment.

### 🔹 Task
* Process a raw customer service dataset with significant data quality issues (including over 20,000 blank survey responses).
* Isolate underperforming regional centers, communication channels, and common call categories using exploratory data analysis.
* Build a 3-page, fully interactive business dashboard that seamlessly translates complex granular data into immediate executive insights.

### 🔹 Action
* **Data Engineering:** Developed a preprocessing script in **Python (Pandas)** to handle missing values logically, normalize column formats, handle timestamps, and output clean datasets for downstream BI modeling.
* **Metric Formulation:** Engineered explicit **DAX measures** to track true baseline performance, including precise Average CSAT scores ($5.55/10$) and Survey Response Rates ($37.25\%$).
* **Root-Cause Analysis:** Isolated **Chicago/IL** as the lowest-performing hub ($5.48$ CSAT). Designed a dual-axis column and line chart to uncover a major operational conflict: while *Billing Questions* drove the highest ticket volume (**3,855 calls**), automated *Chatbots* and *Email* channels were bottlenecking resolutions with high-friction handling loops, yielding the lowest satisfaction scores ($5.39$ and $5.18$ CSAT respectively).

### 🔹 Result
Delivered an executive-ready strategic dashboard that provides leadership with precise operational direction:
1. **Chatbot Overhaul:** Recommended a logic rewrite to bypass automated scripts and immediately route *Service Outage* tickets to live phone agents, who hold the center’s highest performance score (**5.73 CSAT**).
2. **Deflection Strategy:** Proposed a targeted self-service "Quick-Pay FAQ" SMS workflow to deflect heavy volumes away from the overloaded billing queue.
3. **Quality Assurance Audit:** Formulated targeted training directives focused on the Chicago email support team to bridge the performance gap between asynchronous chat channels and phone systems.

---

## 🖥️ Dashboard Architecture & Interface

### 📊 1. Executive Summary Dashboard (Page 1)
Provides a high-level overview of global call volumes, average baseline satisfaction, survey response trends, and a geographical performance ranking.
![Executive Summary](Executive_Summary_Page1.png)

### 🔍 2. Operational Deep-Dive: Chicago/IL (Page 2)
An interactive drill-down canvas isolating the root causes of underperformance in Chicago by mapping volume against channel satisfaction and customer sentiment against call duration.
![Chicago Deep-Dive](Chicago_Deep_Dive_Page2.png)

### 💡 3. Strategic Insights & Action Plan (Page 3)
A data-driven consulting summary translating analytical patterns into business directives and structured operational recommendations for management.
![Strategic Action Plan](Strategic_Action_Plan_Page3.png)

---

## 📁 Repository Structure
* `Call_Center_Analysis.ipynb`: Jupyter Notebook detailing the data cleaning, data type casting, and exploratory analysis phase.
* `Call_Center_Performance_Dashboard.pbix`: The complete Power BI Desktop file containing the data model, DAX measures, and visual components.
* `*.png`: High-resolution application screenshots for immediate documentation.

---
*Note: To test the interactive page navigation buttons locally in Power BI Desktop, remember to hold **Ctrl + Click** on the sidebar menu icons.*
