# Work Breakdown Structure (WBS) & Agile Backlog

**Project:** Global Tech Layoffs vs. The AI Investment Boom  
**Author:** Athulya Peshali Herath  
**Framework:** Agile Scrum (3 Sprints)  

---
## 1. Work Breakdown Structure (WBS)
```text
1. Global Tech Layoffs vs. AI Boom Project
   ├── 1.1 Project Management & Business Analysis (Phase 1)
   │   ├── 1.1.1 Create Business Requirements Document (BRD)
   │   ├── 1.1.2 Create Requirements Traceability Matrix (RTM)
   │   ├── 1.1.3 Formulate WBS and Risk Register
   │   └── 1.1.4 Initialize GitHub Repository Structure
   ├── 1.2 Data Engineering & Pipeline Development (Phase 2)
   │   ├── 1.2.1 Source Raw Datasets (Layoffs & Funding Data)
   │   ├── 1.2.2 Build Data Pipeline Script (pandas/Python)
   │   ├── 1.2.3 Handle Missing Values, Text Normalization, and Dates
   │   └── 1.2.4 Export Processed CSV Data to /data/processed/
   ├── 1.3 Data Analytics & Power BI Modeling (Phase 3)
   │   ├── 1.3.1 Build Star Schema Data Model
   │   ├── 1.3.2 Write Custom DAX Measures
   │   └── 1.3.3 Design Interactive Report Canvas & UI Layout
   └── 1.4 Portfolio Integration & GitHub Release (Phase 4)
       ├── 1.4.1 Capture Dashboard Preview Assets
       ├── 1.4.2 Finalize Portfolio README.md
       └── 1.4.3 Embed Live Interactive Power BI Link

```
---

## 2. Sprint Backlog & User Stories

### Sprint 1: Setup & Business Scaffolding
* **US-01 (BA):** As a Business Analyst, I want to define clear project requirements so that the data pipeline and dashboards meet stakeholder objectives.

### Sprint 2: Data Pipeline & Data Modeling
* **US-02 (SE):** As a Developer, I want to write a Python script that cleans raw layoff and VC funding data so that the resulting dataset is structured for analysis.
* **US-03 (DA):** As an Analyst, I want to establish a Star Schema in Power BI so that data can be filtered efficiently across dimensions.

### Sprint 3: Visualization & Portfolio Deployment
* **US-04 (DA/BA):** As an Executive, I want an interactive dashboard so I can slice layoff data by year, sector, and geographic region alongside AI investment growth.

---

## 3. Project Risk Register

| Risk ID | Risk Category | Risk Event Description | Impact | Mitigation Strategy |
| :--- | :--- | :--- | :--- | :--- |
| **RSK-01** | Data Quality | Inconsistent company naming across datasets. | Medium | Standardize text casing and trimming in Python ETL script. |
| **RSK-02** | Technical | GitHub Markdown strips embedded `<iframe>` tags. | Low | Use clickable preview image badge linked to public Power BI report URL. |
| **RSK-03** | Scope | Data pipeline scope expansion. | Medium | Lock scope to static date-range batch processing (2022–2026). |