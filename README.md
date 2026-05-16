# Clinical Data Analysis: Two-Way ANOVA on Diabetes Hospitalization Lengths

## Project Overview
This repository contains a statistical analysis of real-world clinical data (RWD) to understand how demographic and clinical factors intersect. 

Using the **Diabetes 130-US Hospitals (1999–2008) Dataset** from the UCI Machine Learning Repository, this analysis evaluates the joint impact of a patient's demographic background and their metabolic metrics on overall turnaround times in acute care.

### Research Question: How do the race of the patient (race) and their A1C test results (A1Cresult) jointly influence the duration of their hospital stay (time_in_hospital)?

-  **Independent Variable 1 (iV1):** Patient Race (`race`)
        - (Race - race): Caucasian, Asian, African American, Hispanic, Other
-  **Independent Variable 2 (iV2):** HbA1c Test Results (`A1Cresult`)
        - (A1C test result - a1c): >8%, 7%, Normal, None (not measure)
-  **Dependent Variable (DV):** Duration of hospital stay (`time_in_hospital` in days)

## Statistical Methodology
-   **Two-Way ANOVA:** To isolate the main effects between demographics and metabolic metrics.
-   **Post-Hoc Analysis:** Utilized Tukey’s Honestly Significant Difference (HSD) testing.

## Tech Stack
- Data Engineering: `pandas`, `ucimlrepo`
- Statistical Modeling: `scipy.stats`, `statsmodels`
