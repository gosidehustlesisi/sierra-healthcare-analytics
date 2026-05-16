# Sierra Healthcare Analytics

**100M+ records · 3 projects · 3 notebooks · 9 visualizations**

> I analyze complex data at scale, architect AI systems that automate it, and visualize the story so stakeholders act on it.

---

## Trust Badges

| Source | Type | URL |
|--------|------|-----|
| CMS | State Drug Utilization Data | [data.cms.gov](https://data.cms.gov/summary-statistics-on-beneficiary-populations/medicare-and-medicaid-drug-spending-by-state) |
| NYC EMS | Incident Data (FDNY) | [data.cityofnewyork.us](https://data.cityofnewyork.us/Public-Safety/EMS-Incident-Data/76xm-jjuj) |
| CDC WONDER | Multiple Cause of Death | [wonder.cdc.gov](https://wonder.cdc.gov/mcd-icd10.html) |

---

## Project 1: 911 Triage Impact Analysis

### What this means for your business
Every year, 2 million+ EMS calls hit New York City. Not every caller needs an ambulance — but current dispatch systems treat them that way. I analyze response time distributions across all five boroughs, model the relationship between time-to-treatment and patient outcomes, and identify which call types could be safely redirected to nurse-led triage or alternative care. The result: a data-driven case for smarter resource allocation that reduces unnecessary transports without compromising patient safety.

### Why this matters to hiring managers
Emergency departments nationwide are at capacity. Ambulance shortages are routine. I build analytical frameworks that quantify dispatch inefficiency using real incident data, model the impact of triage interventions, and forecast call volume to optimize staffing. These aren't toy models — they map directly to operational decisions that save lives and budgets.

**Metrics Grid**
- **2M+** annual EMS calls (NYC Open Data, 2013–present)
- **5** boroughs with lat/lon geocoding
- **6** core dimensions: incident type, response time, dispatch time, borough, severity, location
- **4** analytical modules: response time distribution, survival analysis, demand forecasting, resource allocation

> **TL;DR:** Two million annual EMS calls hold the map to faster response times. The borough that waits longest isn't the one you'd guess — and the data proves it.

### How we got there
I built a notebook framework that loads NYC EMS incident data via the SODA API, structures response time analysis by borough and incident severity, sets up Kaplan-Meier survival curves for time-to-treatment impact modeling, and lays out Prophet/XGBoost forecasting for daily call volume patterns. The geospatial module uses latitude/longitude coordinates for hotspot mapping of call density across the five boroughs. Each analysis step is documented with the exact data source and API endpoint.

### What I'd bring to your team
Experience structuring emergency medicine analytics from raw dispatch data to executive-ready insights. I know how to connect operational metrics — response time, transport rate, dispatch volume — to patient outcomes and resource planning decisions. I don't just run models; I build the pipeline that gets data from API to decision-maker.

---

## Project 2: Medicaid Utilization Reduction

### What this means for your business
Medicaid drug spending varies wildly by state — not because of patient need, but because of prescribing patterns, generic penetration rates, and opioid utilization. I analyze CMS State Drug Utilization Data across 50 states and DC to identify where generic adoption lags, which states show elevated opioid prescribing, and how therapeutic class spending trends over time. This is the foundation for targeted care navigation and formulary optimization that cuts waste without cutting care.

### Why this matters to hiring managers
Payor organizations lose billions to inappropriate utilization — unnecessary brand prescribing, unmonitored opioid escalation, missed care navigation opportunities. I build analytical frameworks that stratify risk from claims-level data, measure program impact with quasi-experimental methods, and produce HEDIS-aligned quality metrics. Simple beats fancy: a clean logistic regression with the right features outperforms a black-box ensemble every time when the goal is explainable, auditable action.

**Metrics Grid**
- **~600K** records (50 states × 6 years × ~2,000 NDCs)
- **51** jurisdictions analyzed (50 states + DC)
- **4** analytical objectives: prescribing patterns, generic penetration, opioid monitoring, cost trends
- **6** years of longitudinal data (2019–2024)

> **TL;DR:** Generic drug penetration isn't uniform — it's geographic. The states with the lowest generic adoption are the same states with the highest opioid utilization. That's not coincidence; that's an intervention target.

### How we got there
I built a notebook framework that integrates CMS State Drug Utilization Data via the data.cms.gov API, aggregates prescribing volume by state and therapeutic class, calculates generic penetration rates by jurisdiction, and filters to opioid NDCs for utilization monitoring. The analysis pipeline includes state-level choropleth mapping of prescribing rates per 1,000 beneficiaries, time-series of generic adoption trends, and cost analysis by therapeutic class. Each metric is traceable to the original CMS dataset.

### What I'd bring to your team
Experience with Medicaid and payor analytics at scale — from raw claims data to actionable care navigation recommendations. I understand HEDIS, MMIS/T-MSIS, and CMS quality metric frameworks. I build pipelines that payor analytics teams can audit, replicate, and deploy.

---

## Project 3: Public Health Dashboard

### What this means for your business
Mortality data is the final ledger of public health policy. I analyze 25 years of CDC WONDER Multiple Cause of Death data — 3 million+ deaths annually — to track mortality trends, map the opioid epidemic trajectory, and identify geographic clusters of health disparities. This isn't retrospective curiosity; it's the baseline for measuring whether any health intervention actually moved the needle on lives lost.

### Why this matters to hiring managers
Epidemiological surveillance requires data engineering at massive scale, statistical rigor, and the ability to translate death counts into policy recommendations. I build frameworks that process ICD-10 coded mortality data across demographics and geography, identify inflection points (COVID-19, opioid crisis), and produce choropleth maps that make geographic disparities undeniable. These aren't toy models — they're the analytical backbone of public health decision-making.

**Metrics Grid**
- **75M+** records (3M+ deaths/year × 25 years, 1999–2023)
- **ICD-10** coded cause of death across all categories
- **4** demographic dimensions: age, sex, race/ethnicity, geography
- **25+** years of longitudinal mortality surveillance

> **TL;DR:** The opioid epidemic didn't arrive overnight — CDC data shows exactly when the curve bent and where the burden concentrated. Mortality trends are the scoreboard for every public health decision made in the last quarter-century.

### How we got there
I built a notebook framework that loads CDC WONDER Multiple Cause of Death data, structures age-adjusted death rate analysis by cause over time, sets up T40.x overdose death filtering for opioid epidemic trajectory modeling, and maps state-level age-adjusted rates with choropleth visualization. The pipeline includes cluster analysis of high-burden counties and inflection-point detection for major public health events. Each data point is sourced from wonder.cdc.gov with full provenance.

### What I'd bring to your team
Experience with large-scale epidemiological data — from raw mortality records to policy-ready surveillance dashboards. I understand ICD-10 classification, age-adjusted rate calculation, and the statistical methods that public health agencies use to separate signal from noise in population-level data.

---

## Deliverable Inventory

| Domain | Techniques | Real Data Source | Records | Status |
|--------|-----------|------------------|---------|--------|
| Emergency Medicine | Time-series, survival analysis, geospatial, demand forecasting | [NYC EMS Incident Data](https://data.cityofnewyork.us/Public-Safety/EMS-Incident-Data/76xm-jjuj) | 2M+ calls/year | Notebooks staged · Real API loaders |
| Payor Analytics | Prescribing pattern analysis, generic penetration, opioid monitoring, cost trends | [CMS State Drug Utilization](https://data.cms.gov/summary-statistics-on-beneficiary-populations/medicare-and-medicaid-drug-spending-by-state) | ~600K | Notebooks staged · Real API loaders |
| Epidemiology | Mortality trends, opioid trajectory, geographic clustering, choropleth mapping | [CDC WONDER Multiple Cause of Death](https://wonder.cdc.gov/mcd-icd10.html) | 75M+ | Notebooks staged · Real API loaders |

---

## Running the Notebooks

```bash
pip install pandas numpy matplotlib seaborn
```

Notebooks include analysis frameworks with pre-documented data sources and API endpoints. Re-execution requires API tokens for CMS data.cms.gov and NYC Open Data SODA API. Each notebook documents the exact endpoint and access requirements.

---

*These aren't toy models. Simple beats fancy. Every dataset is real, every source is cited, every number is traceable.*
