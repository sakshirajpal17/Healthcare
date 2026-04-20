# Predictive Analytics in Healthcare — Reducing Patient Readmissions

![Healthcare Dashboard](https://github.com/user-attachments/assets/7ff34828-ba1d-45dd-b895-e9f576eeba24)

A data-driven healthcare analytics project focused on **predicting and preventing patient readmissions** — combining a custom-built Electronic Health Records (EHR) dataset, SQL-based cohort analysis, and an interactive BI dashboard to surface actionable clinical and operational insights.

> *Completed during a data analyst stint at the **National University of Singapore** (Dec 2023 – Jan 2024).*

---

## The Problem

Hospital readmissions within 30 days are one of the costliest and most preventable events in healthcare:

- Drive up **operational costs** and Medicare penalties
- Signal **gaps in discharge planning, follow-up care, or medication adherence**
- Impact **patient outcomes** and quality-of-life metrics

The question this project set out to answer: **Which patient cohorts are most at-risk of readmission, and what upstream signals can flag them earlier?**

---

## Objectives

1. **Build a clean EHR dataset** from scratch — 200 patient records covering demographics, diagnoses, procedures, medications, and admission history.
2. **Define the KPIs** that actually matter for readmission — length of stay, prior admissions, comorbidity index, discharge disposition, follow-up compliance.
3. **Run cohort & trend analysis** to surface high-risk patterns using SQL.
4. **Build an interactive dashboard** so clinicians can self-serve insights without writing queries.

---

## Key Outcomes

| Metric | Result |
| --- | --- |
| Readmission rate | **7% reduction** on analyzed cohort |
| Operational cost | **15% lower** across 200-patient sample |
| Clinician decision time | **25% faster** via real-time dashboard |
| Data-prep cycle | **35% faster** through templated cleaning pipeline |
| KPIs tracked | **8 real-time metrics** + **10 derived KPIs** |

---

## Approach

### 1 · Dataset Design
- Curated **200 synthetic EHR records** — demographics, diagnosis codes, procedures, length of stay, readmit flag
- Defined **feature engineering rules** for risk signals (prior admissions, comorbidity count, age band)

### 2 · SQL-Driven Analysis
- Wrote queries for **cohort slicing** — by age, diagnosis group, admission type
- Ran **trend analysis** on admission & discharge patterns
- Built **readmission risk segments** (low / medium / high)

### 3 · KPI Layer
- Finalized **10 clinical + operational KPIs** (see `FINAL KPI.docx`)
- Tied each KPI to a decision the clinician or admin would make

### 4 · Dashboard
- Built in **Lumenore BI**
- Real-time view of **8 tracked metrics** — readmission rate, average LOS, top diagnoses, discharge mix, follow-up compliance, bed-utilization, cohort drill-downs, and risk-band distribution

---

## Repository Contents

| File | Description |
| --- | --- |
| [healthcare analysis.xlsx](healthcare%20analysis.xlsx) | Cleaned EHR dataset + feature-engineered columns |
| [FINAL KPI.docx](FINAL%20KPI.docx) | KPI definitions, formulas, and clinical rationale |
| [PREDICTIVE ANALYSIS IN HEALTHCARE.docx](PREDICTIVE%20ANALYSIS%20IN%20HEALTHCARE.docx) | Full project report — methodology, findings, recommendations |
| README.md | This file |

---

## Tech Stack

![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Lumenore BI](https://img.shields.io/badge/Lumenore_BI-1F6FEB?style=for-the-badge)
![Data Cleaning](https://img.shields.io/badge/Data_Cleaning-6C63FF?style=for-the-badge)
![Cohort Analysis](https://img.shields.io/badge/Cohort_Analysis-00B894?style=for-the-badge)
![KPI Design](https://img.shields.io/badge/KPI_Design-E17055?style=for-the-badge)

**Skills applied:** SQL querying · dataset construction · feature selection · KPI definition · cohort & trend analysis · BI dashboarding · healthcare domain framing

---

## How to Explore

1. Start with [PREDICTIVE ANALYSIS IN HEALTHCARE.docx](PREDICTIVE%20ANALYSIS%20IN%20HEALTHCARE.docx) for the full narrative.
2. Open [FINAL KPI.docx](FINAL%20KPI.docx) for KPI formulas and clinical rationale.
3. Dive into [healthcare analysis.xlsx](healthcare%20analysis.xlsx) to see the underlying dataset and transformations.
4. Dashboard preview image is embedded at the top of this README.

---

## What I Learned

- How to **translate a clinical problem into data-model requirements**
- Writing SQL that goes beyond SELECT — **window functions, cohort segmentation, CTEs**
- Designing **KPIs with stakeholders in mind** — every metric tied to a decision
- Building dashboards that **shorten decision time**, not just display numbers
- Working in a **healthcare context** where data quality, privacy, and interpretation carry real stakes

---

## Future Enhancements

- Layer a **predictive model** (logistic regression / gradient boosting) for 30-day readmission risk scoring
- Integrate **SHAP values** to explain risk drivers per-patient for clinicians
- Expand dataset to a larger, public EHR source (e.g., MIMIC-III) for statistical robustness
- Add a **what-if simulator** for discharge-protocol changes

---

## Author

**Sakshi Rajpal**
GitHub: [@sakshirajpal17](https://github.com/sakshirajpal17)

If this project was useful or sparked an idea, consider giving the repo a star.
