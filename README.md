# Audit Support & Analytics — Python Toolkit

I provide **full technical and analytical support to internal audit functions**, combining traditional audit methodology with data analytics and automation. Below is a summary of the audit areas I cover and the tools I have developed throughout my professional experience.

> Code access is restricted. To request it, open an [Issue](https://github.com/jaimegarciasdr9/audit-codes-python-info/issues/new?title=Access+Request&body=Name%3A+%0AReason%3A+) and I will review it promptly.

---

## What I Do

I support internal audit teams across the full audit cycle — from planning and risk assessment to fieldwork, reporting and follow-up. My work combines technical rigour with automation to make audit procedures more efficient, reproducible and defensible.

**Areas of expertise:**

- **Credit Risk Model Validation** — Independent replication and review of PD, LGD and EAD models under IFRS 9 / CECL frameworks. Assessment of reserve calculations and model assumptions.
- **Asset Management Audits** — Verification of net asset values (NAV), investment limit controls, valuation of illiquid assets, and review of fund management delegation agreements.
- **Regulatory & Compliance Audits** — AML/AMLD reviews, KYC process audits, sanctions screening controls, and supervisory recommendation follow-up (e.g. Banco de España).
- **IT & Cybersecurity Audits** — Logical access controls, change management, business continuity plans, SIEM and information security reviews.
- **Internal Control Reviews** — Risk appetite framework assessment, stress testing processes, market and credit risk metrics.
- **Continuous Audit & Monitoring** — Ongoing plan-of-action tracking, implementation of audit recommendations, and structured reporting to Audit Committees.
- **Data Analytics for Audit** — Automated data extraction, document processing, analytical procedures and audit evidence management using Python.

---

## Available Code Projects

The following scripts are available in the private repository. Each one is production-ready and has been used in real audit engagements.

---

### `ifrs9-riesgo-credito/` — IFRS 9 Credit Risk Models

Independent replication of credit risk models for IFRS 9 audit purposes (LEVAs methodology).

| Script | What it does |
|---|---|
| `01_replica_PD_GT.py` | Replicates the client's **Probability of Default (PD)** model using logistic regression. Validates coefficients, calibration and discriminatory power. |
| `02_replica_LGD_GT.py` | Replicates the **Loss Given Default (LGD) / Severity** model. Compares outputs against the entity's own model results. |
| `03_calculo_reservas.py` | Calculates **IFRS 9 provisions** from PD and LGD outputs. Produces stage-by-stage reserve estimates for comparison with reported figures. |

**Stack:** Python · pandas · numpy · statsmodels  
**Use case:** Credit risk model audit, IFRS 9 independent validation, regulatory review support.

---

### `nav-valores-liquidativos/` — NAV Verification & Fund Data

Automated extraction and verification of net asset values (NAV) for investment funds from multiple official and market sources.

| Script | What it does |
|---|---|
| `get_nav_cnmv.py` | Fetches NAV data directly from the **CNMV** (Spain's financial regulator) registry. |
| `nav_todos.py` | Aggregates NAV for a full portfolio of funds by combining **Yahoo Finance + CNMV** sources. |
| `nav_yahoo.py` | Queries NAV by **ISIN** from Yahoo Finance. Handles multiple funds in batch. |
| `yahoo_finance.py` | Shared connection layer and utilities for the Yahoo Finance API. |
| `valor_liquidativo.py` | Computes the **net asset value** from raw fund data. |
| `get_nav_31032026.py` | Point-in-time NAV extraction at a specific audit date for evidence-gathering purposes. |

**Stack:** Python · yfinance · requests · pandas  
**Use case:** Asset management audits, NAV verification, investment fund controls.

---

### `utils/` — General Audit Utilities

| Script | What it does |
|---|---|
| `extraer_dnis.py` | Extracts and counts **DNI / NIE identity numbers** from text-selectable PDF documents. Useful for KYC reviews, client file audits and data completeness testing. |

**Stack:** Python · pdfplumber · re  
**Usage:** `python extraer_dnis.py report.pdf`

---

### `audit-dashboard.html` — Audit Committee Dashboard

An interactive **management control dashboard** used as the standard reporting format presented to the Audit Committee. Covers roadmap, control status, team assignments and meeting calendar.

> **[➜ Open Dashboard](audit-dashboard.html)**  
> No installation required — opens directly in any browser.

---

## Request Access

The source code is private. To request access, open an Issue describing your name and intended use — I will review and respond within 24 hours.

**[➜ Open an Access Request](https://github.com/jaimegarciasdr9/audit-codes-python-info/issues/new?title=Access+Request&body=Name%3A+%0AReason%3A+)**
