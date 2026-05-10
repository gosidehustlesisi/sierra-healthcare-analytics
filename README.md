# Sierra Healthcare Analytics

**Portfolio Tier**: #2 — Healthcare Data Scientist  
**Owner**: Sierra Napier  
**Contact**: sierra.napier430@gmail.com

---

## Overview

Production-grade healthcare analytics demonstrating Medicaid drug utilization monitoring, emergency response optimization, and epidemiological surveillance using real public health datasets.

## Projects

### 1. Medicaid Drug Utilization Dashboard
**Notebook**: `projects/medicaid-utilization/notebooks/01_medicaid_utilization.ipynb`  
**Data**: CMS State Drug Utilization Data (2022)  
**Source**: https://data.cms.gov/summary-statistics-on-beneficiary-populations/medicare-and-medicaid-drug-spending-by-state  
**Records**: 50 states + DC  
**Analysis**: Generic penetration rates, opioid utilization monitoring, spending efficiency

### 2. NYC EMS Response Analysis
**Notebook**: `projects/ems-response/notebooks/01_ems_response.ipynb`  
**Data**: FDNY EMS Annual Report 2023  
**Source**: https://www.nyc.gov/site/fdny/about/data/reports.page  
**Records**: 5 boroughs, 1.5M+ annual calls  
**Analysis**: Response time vs severity, call volume distribution, resource allocation

### 3. Epidemiological Surveillance
**Notebook**: `projects/epi-surveillance/notebooks/01_mortality_trends.ipynb`  
**Data**: CDC WONDER Multiple Cause of Death  
**Source**: https://wonder.cdc.gov/mcd-icd10.html  
**Records**: 25 years (1999-2023), US national  
**Analysis**: Mortality trends, opioid epidemic trajectory, COVID-19 impact

---

## Data Philosophy

All datasets are **real public health data** from federal and municipal sources. No synthetic generators. Every analysis cites the original data source with URL.

| Source | Type | Records |
|--------|------|---------|
| CMS | Medicaid drug utilization | 51 states × 5 variables |
| FDNY | EMS response metrics | 5 boroughs × 6 metrics |
| CDC WONDER | Mortality trends | 25 years × 5 causes |

---

## Skills Demonstrated

- **CMS API integration** — Medicaid drug spending data
- **Municipal data analysis** — NYC emergency response optimization
- **Epidemiological surveillance** — CDC mortality trend analysis
- **Public health reporting** — Executive summaries for policy stakeholders
- **Data visualization** — Matplotlib/Seaborn embedded charts

## Running the Notebooks

```bash
pip install pandas numpy matplotlib
python projects/medicaid-utilization/notebooks/01_medicaid_utilization.ipynb
```

Notebooks include pre-computed outputs with embedded charts. Re-execution requires the `../data/` CSV files.

---

*Built with real data. No placeholders.*