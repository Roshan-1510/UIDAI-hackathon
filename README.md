

# Age-wise Aadhaar Enrolment Analysis at Pincode Level

## Overview
This project analyzes Aadhaar enrolment patterns at the pincode-day level using aggregated administrative data provided for a Government of India data hackathon. The objective is to identify meaningful patterns, anomalies, and monitoring indicators that can support evidence-based administrative decision-making.

The analysis focuses on enrolment distribution across age groups, geographic concentration, temporal trends, and the identification of statistically unusual activity patterns using simple, interpretable indicators.

---

## Problem Statement
How can aggregated Aadhaar enrolment data be used to identify structural patterns and early warning signals in enrolment activity across regions and age groups, without overclaiming causality or individual-level behavior?

---

## Dataset Summary
- **Source:** UIDAI Hackathon Dataset  
- **Unit of Analysis:** Date × Pincode  
- **Geographic Coverage:** India (State, District, Pincode)  
- **Time Coverage:** As provided in the dataset  
- **Key Variables:**
  - age_0_5
  - age_5_17
  - age_18_greater
- **Derived Variables:**
  - total_enrol
  - activity volume tiers (percentile-based)
  - child under-focus indicator

---

## Methodology
- Data cleaning focused on schema validation, null handling, and grain preservation.
- Percentile-based thresholds were used to define normal vs. unusually low/high enrolment activity.
- Simple, interpretable indicators were constructed to support monitoring and administrative review.
- No individual-level inference or causal claims are made.

---

## Key Insights
- Aadhaar enrolment activity is highly uneven across states, indicating geographic concentration of system load.
- At the pincode-day level, enrolments are typically low, with most observations falling within a narrow range.
- Statistically unusual enrolment patterns are concentrated in specific regions and time periods rather than being system-wide.
- A subset of low-volume areas shows persistently low child enrolment share, warranting targeted administrative review.

---

## Impact & Applicability
- Enables targeted monitoring instead of blanket interventions.
- Supports early identification of regions requiring operational or outreach review.
- Indicators are simple, transparent, and feasible to operationalize within existing administrative systems.

---

## Limitations
- Data is aggregated; no individual-level conclusions can be drawn.
- Capacity, staffing, infrastructure, and demand-side variables are not available.
- Indicators highlight areas for review but do not establish root causes.

---

## Repository Contents
- `notebooks/aadhaar_analysis_final.ipynb` – Final, submission-ready analysis notebook  
- `reports/Aadhaar_Enrolment_Analysis_Report.pdf` – Exported report for quick review  

---

## How to Run
1. Open the notebook in Google Colab or Jupyter.
2. Install dependencies listed in `requirements.txt`.
3. Run the notebook top-to-bottom.

---

## License
This project is submitted for evaluation purposes under the hackathon guidelines.
