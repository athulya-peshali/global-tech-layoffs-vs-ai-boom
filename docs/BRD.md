# Business Requirements Document (BRD)

**Project Title:** Global Tech Layoffs vs. The AI Investment Boom (2022–2026)  
**Document Version:** 1.0.0  
**Author:** Athulya Peshali Herath (Software Engineering & Business Analysis)  
**Status:** Approved

---

## 1. Executive Summary

Between 2022 and 2026, the technology sector experienced significant headcount reductions alongside rapid capital deployment into Artificial Intelligence (AI). This project provides a quantitative analysis to determine whether tech layoffs correlate with macroeconomic contraction or reflect a strategic reallocation of corporate capital directly into AI infrastructure and R&D.

---

## 2. Business Problem & Scope

- **Problem:** Executive leadership and workforce strategy teams lack integrated visibility into whether headcount reductions are cyclical cost-cutting measures or permanent structural replacements driven by enterprise AI automation.
- **In-Scope:**
  - Ingestion and cleaning of global layoff records (2022–2026).
  - Analysis of quarterly venture capital trends comparing AI-native vs. Non-AI tech sectors.
  - Interactive Power BI star schema dashboard with custom DAX KPIs.
- **Out-of-Scope:** Real-time streaming APIs and individual employee PII analysis.

---

## 3. User Personas

- **Chief Strategy Officer:** Needs high-level trend visuals comparing YoY headcount reductions against AI capital expenditures.
- **Talent & HR Director:** Needs industry treemaps and geographic maps to assess sector vulnerability and talent displacement.
- **Venture Capital Analyst:** Wants to track quarterly venture funding growth share across sub-sectors.

---

## 4. Requirements Traceability Matrix (RTM)

| Req ID     | Business Objective                            | Source Dataset       | Deliverable Target        |
| :--------- | :-------------------------------------------- | :------------------- | :------------------------ |
| **OBJ-01** | Quantify total tech headcount cut (2022–2026) | `Layoffs.fyi`        | Power BI Summary KPI Card |
| **OBJ-02** | Track AI vs. Non-AI capital trends            | Venture Funding Data | Dual-Axis Trend Visual    |
| **OBJ-03** | Map geographic impact concentrations          | `Layoffs.fyi`        | Geographic Bubble Map     |
| **OBJ-04** | Automate ETL data transformation              | Python / Pandas      | `src/etl_pipeline.py`     |
