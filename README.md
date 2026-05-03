# Multi-Partner Reporting Platform

> Automated reporting platform serving 20+ global airline partners — each with partitioned, zero-cross-visibility views of their own operational data.

![Stack](https://img.shields.io/badge/SQL-Automation-0C447C?style=flat-square&labelColor=E6F1FB)
![Stack](https://img.shields.io/badge/Spotfire-Dashboards-633806?style=flat-square&labelColor=FAEEDA)
![Stack](https://img.shields.io/badge/Python-Pipelines-27500A?style=flat-square&labelColor=EAF3DE)

---

## 📌 Overview

A multi-tenant automated reporting platform built for United Airlines' global partner ecosystem. Each of 20+ international partners receives automated, scheduled reports with visibility into their own operational data only — strict data partitioning ensures zero cross-partner data leakage.

**Role:** Sole analyst and developer  
**Scale:** 20+ global partners · Automated monthly + ad-hoc reporting  
**Outcome:** 90% reduction in manual reporting effort

---

## 🎯 Business Problem

| Before | After |
|---|---|
| Reports manually prepared per partner | Fully automated per-partner delivery |
| Hours of analyst effort per cycle | Zero analyst effort for standard reports |
| Risk of data cross-contamination | Strict SQL-level partitioning |
| No self-serve capability | Partners receive data on schedule |

---

## ⚙️ Tech Stack

| Component | Technology |
|---|---|
| Reporting dashboards | Spotfire |
| Data pipelines | SQL · Python |
| Partitioning logic | Parameterized SQL by partner ID |
| Scheduling | Automated refresh cadence |

---

## 🏗️ Key Design Decisions

### Data partitioning
Each partner's data view is generated via parameterized SQL queries filtered strictly by partner ID. No partner can access another's data — partitioning is enforced at the query level, not the application level.

### Automated delivery
Reports are auto-generated and distributed on a scheduled cadence without analyst intervention. Exception handling flags any data quality issues before delivery.

### Scalability
Adding a new partner requires only a new partner ID configuration — no new pipeline development needed.

---

## 📈 Outcomes

- **Partners served:** 20+ global airline partners
- **Manual effort eliminated:** ~90%
- **Data incidents:** Zero cross-partner data leakage
- **Analyst time freed:** Redirected to higher-value AI/automation projects

---

## 🔒 Note

Built and deployed within United Airlines' internal operations environment. Source code and data are confidential.

---

## 👤 Author

**Apoorv Chauhan**  
📧 apoorvchauhan381@gmail.com · 💼 [LinkedIn](https://linkedin.com/in/apoorv-chauhan-8a8865198)
