## Project 2: 911 Triage Impact Analysis

**Context:** Emergency medicine analytics inspired by DC's "Right Care, Right Now" 911 Nurse Triage program (2019–2022).

**Dataset:**
- [DC Open Data — EMS Dispatches](https://opendata.dc.gov/)
- [NHTSA FARS](https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars)
- [Census ACS](https://data.census.gov/)

**Objective:** Evaluate the impact of nurse-led 911 triage on ambulance utilization, ED crowding, and patient outcomes using quasi-experimental methods.

**Techniques:**
- Interrupted time series (ITS) analysis
- Difference-in-differences (DiD) with synthetic control
- Geospatial hotspot mapping of call patterns
- Propensity score weighting for triage-eligible vs. ineligible calls

**Business Impact:**
- Ambulance dispatch rates: 97% → 56% (41pp reduction for triage-eligible calls)
- Ambulance transports: 73% → 45% (28pp reduction)
- Program scaled to 24/7 operation, 50,000+ calls triaged annually

**Files:**
- `notebooks/01_dispatch_data_exploration.ipynb`
- `notebooks/02_its_analysis.ipynb`
- `notebooks/03_did_synthetic_control.ipynb`
- `notebooks/04_geospatial_hotspots.ipynb`
- `src/preprocess.py`
- `src/its_model.py`
- `src/did_model.py`
- `dashboard/triage_dashboard.py`

**Status:** 🔧 In development
