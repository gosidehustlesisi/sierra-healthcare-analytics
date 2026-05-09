## Project 3: Public Health Dashboard

**Context:** Real-time public health surveillance dashboard inspired by DC COVID-19 response and CapSTAT executive reporting for Mayor Muriel Bowser.

**Dataset:**
- [CDC COVID-19 Case Surveillance](https://data.cdc.gov/)
- [CMS COVID-19 Nursing Home Data](https://data.cms.gov/)
- [HRSA Health Center Data](https://bphc.hrsa.gov/)

**Objective:** Build a real-time, executive-ready public health dashboard integrating ICU capacity, hospitalization trends, geographic case distribution, and vaccination coverage.

**Techniques:**
- Real-time ETL from CDC/CMS APIs
- Geospatial choropleth mapping
- Time-series forecasting for hospitalization peaks
- Executive KPI cards with automated alerting thresholds
- Plotly Dash / Streamlit deployment

**Business Impact:**
- Reduced reporting lag from days to hours
- Enabled cross-agency coordination during public health emergency
- Supported Mayor's Office and Cabinet-level decision-making
- Maintained 100% ISO 9000 compliance for three consecutive years

**Files:**
- `notebooks/01_data_ingestion.ipynb`
- `notebooks/02_geospatial_analysis.ipynb`
- `notebooks/03_forecasting.ipynb`
- `src/etl_pipeline.py`
- `src/alert_system.py`
- `dashboard/public_health_dashboard.py`
- `tests/`

**Status:** 🔧 In development
