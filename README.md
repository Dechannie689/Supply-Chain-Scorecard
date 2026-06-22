# Supply Chain Scorecard

![](https://github.com/Dechannie689/SUPPLY-CHAIN-SCORECARD/blob/main/Supply_Chain_Scorecard.png)

An automated supplier evaluation system that aggregates multi-dimensional performance data from ERP and SharePoint survey forms into a weighted scorecard, enabling procurement teams to rank and compare suppliers across eight criteria.

---

## 📌 Overview

Procurement teams managing multiple suppliers often rely on ad-hoc spreadsheets and subjective assessments to evaluate vendor performance. Without a standardized, data-driven scoring model, it is difficult to make consistent sourcing decisions, identify underperforming suppliers early, or track improvement over time.

This project built a pipeline that ingests supplier data from ERP systems and SharePoint survey forms via Fabric Pipeline and Dataflow, stores it in OneLake, and transforms it through Notebooks to produce master files powering a semantic model in Power BI. The scorecard evaluates each supplier across eight weighted dimensions: Delivery, Quality, Finance, Development, Machinery, Communication, Operation, and Sustainability.

---

## 🏗️ Architecture
![](https://github.com/Dechannie689/Supply-Chain-Scorecard/blob/main/Supply%20Chain%20Scorecard.png)

---

## 🛠️ Tech Stack

- **Fabric Pipeline & Dataflow** — ingests ERP exports and SharePoint survey responses into the Lakehouse on a scheduled basis
- **Databricks Notebooks** — performs data quality checks (accuracy scoring, missing range assessment), cleans text/numeric inconsistencies, and builds the master supplier files
- **Microsoft Fabric Lakehouse / OneLake** — stores raw, transformed, and master data in Delta format
- **Azure AD** — identity management across the platform
- **Azure Key Vault** — secure secret and credential management
- **DevOps** — CI/CD collaboration and deployment
- **Microsoft Purview** — data discovery and governance
- **Azure Monitor** — monitoring and cost management
- **Power BI (Semantic Model)** — auto-generates the supplier scorecard with year filter and stacked bar visualization per supplier

---

## 📊 Dashboard & Key Metrics

The dashboard is used by procurement managers and employees to assess and rank suppliers on an annual basis across eight performance dimensions. The stacked bar format lets teams instantly see which criteria drive a supplier's total score, supporting structured supplier development plans and contract renewal decisions.

[View the full dashboard PDF](https://github.com/Dechannie689/Supply-Chain-Scorecard/blob/main/UA_SUPPLY_CHAIN_SCORECARD.pdf)

---

## 📬 Contact

Built by [Thuy Trang](https://www.linkedin.com/in/trangthuynguyen6899/) · trangthuynguyen6899@gmail.com
