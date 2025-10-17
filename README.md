# Clinical-Trial-Patient-Recruitment-and-Adherence-Monitoring-Power-BI-Machine-Learning-Project
Developed a central command center for pharmaceutical trial managers to monitor patient recruitment and adherence in real time. Built ETL pipelines to integrate anonymized data from EDC and EMR systems, designed a star schema data model, and created interactive Power BI to visualize recruitment funnels, site performance, and adherence trends.
# 🧠 Clinical Trial Patient Recruitment and Adherence Monitoring

## 📋 Project Overview
This project focuses on optimizing **clinical trial management** by developing a **central command center** that enables real-time tracking of **patient recruitment, adherence, and dropout risk**.  
It integrates data from multiple sources (EDC and EMR systems), applies machine learning for dropout prediction, and visualizes KPIs through **Power BI dashboards**.

---

## 🚀 Key Objectives
- Monitor recruitment funnels across multiple trial sites.  
- Identify site-level performance bottlenecks.  
- Track patient visit adherence and medication compliance.  
- Predict patients at high risk of dropout using ML.  
- Provide actionable insights via interactive Power BI dashboards.  

---

## 🏗️ Project Architecture
1. **Data Ingestion & Cleaning** – CSV datasets from multiple trial sources.  
2. **ETL & Modeling** – Performed in Power Query and Python to clean, join, and anonymize data.  
3. **Data Modeling** – Designed a Star Schema in Power BI with fact and dimension tables.  
4. **Analytics Layer** – DAX measures for KPIs (enrollment velocity, adherence %, etc.).  
5. **ML Pipeline** – Logistic Regression model (Python, scikit-learn) to predict patient dropout risk.  
6. **Visualization** – Power BI dashboards for Recruitment Funnel, Site Leaderboard, Adherence, and Risk Insights.  

---

## 🧩 Datasets Used
| Dataset | Description |
|----------|--------------|
| **screening.csv** | Patient screening data (screening date, result, reason for failure). |
| **enrollment.csv** | Enrollment and randomization details for each patient. |
| **visits.csv** | Visit-level adherence data (completed/missed visits, medication %, diary submission). |
| **site_metadata.csv** | Metadata about each clinical site (country, target enrollment, site manager, etc.). |

All datasets are **anonymized** to ensure compliance with data protection regulations.

---

## 🤖 Machine Learning Component
**File:** `patient_dropout_risk.ipynb`

- Trained a **Logistic Regression model** using scikit-learn to predict patient dropout risk.  
- Features used: missed visits count, adherence %, site quality score, demographics, etc.  
- Addressed class imbalance using class weighting.  
- Evaluated performance using **ROC AUC, Precision-Recall, and Confusion Matrix**.  
- Exported risk scores as CSV and integrated into Power BI for visualization.

---

## 📊 Power BI Dashboards
**File:** `Clinical_Trial_Dashboard.pbix`

**Dashboard Pages:**
1. **Enrollment Overview:** Target vs. Enrolled, cumulative trends, forecasted completion date.  
2. **Recruitment Funnel:** Conversion rates from screening to randomization.  
3. **Site Performance Leaderboard:** Enrollment velocity, data quality, and query metrics.  
4. **Patient Adherence Dashboard:** Visit and medication adherence patterns.  
5. **Dropout Risk Insights:** At-risk patient list with predictive scores.  

---

## 🔐 Data Compliance & Security
- All datasets are **fully anonymized** (no PHI).  
- Patient IDs replaced with pseudonyms (e.g., `PAT0001`).  
- **Row-Level Security (RLS)** implemented in Power BI for site-based data access.  
- Audit logs maintained for ETL and transformations.  

---

## 🧰 Tools & Technologies
| Category | Tools / Frameworks |
|-----------|-------------------|
| Data Cleaning | Power Query, Python (pandas) |
| Data Modeling | SQL, Power BI Star Schema |
| Visualization | Power BI, DAX |
| Machine Learning | Python, scikit-learn, pandas, NumPy |
| Version Control | GitHub |

---

## 📅 Project Timeline
| Phase | Tasks | Duration |
|-------|--------|----------|
| Week 1 | Data modeling & anonymization | 7 days |
| Week 2 | Power BI dashboards (Recruitment & Leaderboard) | 7 days |
| Week 3 | Adherence analytics & ML model | 7 days |
| Week 4 | Security, RLS, validation & documentation | 7 days |

---

## 🏁 Deliverables
- Cleaned anonymized datasets (`.csv`)  
- Power BI Dashboard (`.pbix`)  
- Dropout risk model (`.ipynb`)  
- Documentation and README  

---

## ✨ Outcomes
✅ Identified recruitment bottlenecks early using funnel analytics.  
✅ Predicted at-risk patients with ML model integration.  
✅ Improved data transparency and compliance in multi-site trials.  
✅ Provided decision-ready dashboards for clinical managers.

---

## 👩‍💻 Author
**Rakshitha B**  
4th Year, B.E. Computer Science  
Government Engineering College, Chamarajanagar  
Volunteer at Youth for Seva | Aspiring Data Analyst / Data Scientist  

📧 *Feel free to connect or collaborate!*  

---
