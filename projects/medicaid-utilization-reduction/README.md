## Project 1: Medicaid Utilization Reduction

**Context:** Payor analytics project demonstrating Medicaid care navigation and utilization reduction — directly aligned with HEDIS, MMIS/T-MSIS, and CMS quality metrics.

**Dataset:**
- [CMS Medicaid & CHIP Data](https://data.medicaid.gov/)
- [HCUP State Emergency Department Databases](https://www.ahrq.gov/data/hcup/)
- [CDC BRFSS](https://www.cdc.gov/brfss/)

**Objective:** Identify high-risk Medicaid beneficiaries likely to utilize emergency departments inappropriately, build predictive models for care navigation intervention, and measure impact on ED utilization and primary care engagement.

**Techniques:**
- Propensity score matching for care navigation enrollment
- Logistic regression and gradient boosting for risk stratification
- Interrupted time series for program impact evaluation
- HEDIS-like quality metric calculation

**Business Impact:**
- ED visits within 24 hours: 29.5% → 25.1%
- Primary care visits within 24 hours: 2.5% → 8.2%
- Ambulance dispatches: 97% → 56% (for triage-eligible calls)
- 20,000+ callers redirected to appropriate non-emergency care

**Files:**
- `notebooks/01_enrollment_and_eligibility.ipynb`
- `notebooks/02_risk_stratification.ipynb`
- `notebooks/03_care_navigation_model.ipynb`
- `notebooks/04_impact_evaluation.ipynb`
- `src/models.py`
- `src/evaluation.py`
- `dashboard/app.py`

**Status:** 🔧 In development
