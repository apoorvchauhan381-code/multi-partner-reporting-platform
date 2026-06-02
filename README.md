# Multi-Partner Reporting Platform

> Partitioned BI reporting system for global airline partners — hundreds of daily users, significantly faster load times.

## 📋 Overview

Built to serve multiple global airline partners, each requiring isolated, zero-cross-visibility reporting on shared operational data. Partners must see only their own data — never another partner's — while the underlying dataset is unified.

The platform uses row-level security and intelligent partitioning to enforce data isolation, combined with query optimisation and caching to handle high daily user volume without performance degradation.

## ⚙️ Architecture

```
Unified Ops Database
        ↓
  Partitioning Layer (row-level security)
        ↓
  Query Optimisation + Caching
        ↓
 Partner A  |  Partner B  |  Partner C  ...  (isolated views)
        ↓
  Spotfire / Power BI Dashboards (per-partner)
```

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Database | PostgreSQL · T-SQL |
| BI / Dashboards | Spotfire · Power BI |
| Security | Row-level security · Parameterised queries |
| Performance | Query optimisation · Intelligent caching |
| Automation | Python · Scheduled refresh |

## 📊 Results

- 👥 Hundreds of daily active users across multiple partners
- ⚡ Significant improvement in dashboard load time via query optimisation
- 🔒 Zero cross-partner data visibility incidents
- 🔄 Fully automated refresh — no manual report generation
- 📉 Drastic reduction in manual reporting effort organisation-wide

## 🗂️ Repository Structure

```
├── partitioning/    # Row-level security and data isolation logic
├── sql/             # Optimised queries, views, and stored procedures
├── caching/         # Caching layer configuration and strategy
├── dashboards/      # Dashboard templates per partner type
├── automation/      # Scheduled refresh and report distribution
├── data/            # Anonymised sample schemas
└── README.md
```

## 🚀 Getting Started

```bash
git clone https://github.com/apoorvchauhan381-code/multi-partner-reporting-platform
cd multi-partner-reporting-platform
pip install -r requirements.txt
cp config.example.yaml config.yaml  # configure partner list and DB connection
python automation/setup_partners.py
```

## 📝 Notes

All partner names and operational data in sample files are anonymised or fictional.
