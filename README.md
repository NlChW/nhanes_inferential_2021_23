# nhanes_inferential_2021_23
# NHANES 2021–2023 Inferential Analytics Project

This repository contains my completed inferential statistics analysis using the NHANES 2021–2023 dataset.  
The project was completed in Google Colab and includes data preparation, cleaning, variable recoding, inferential tests, and interpretation of results.

---

## Contents
- **nhanes_inferential_2021_23.ipynb**  
  Google Colab notebook containing all data preparation steps, analysis code, visualizations, and written interpretations.

---

## Project Overview
This project explores key relationships in the NHANES 2021–2023 dataset using inferential statistics.  
The analyses examine associations and differences across demographic, behavioral, and clinical health measurements.

NHANES data files used:
- Demographics (`DEMO_L.xpt`)
- Physical Activity (`PAQ_L.xpt`)
- Kidney Questionnaire (`KIQ_U_L.xpt`)
- Body Measures (`BMX_L.xpt`)
- Blood Pressure (`BPXO_L.xpt`)
- Vitamin D Lab (`VID_L.xpt`)
- Hepatitis B Lab (`HEPB_S_L.xpt`, if available)

All SAS Transport files were loaded, merged on `SEQN`, cleaned, and transformed for analysis.

---

## Analyses Included
The notebook answers the following required questions:

### **Q1 — Chi-Square Test**
Is there an association between marital status and education level?

### **Q2 — T-Test**
Is there a difference in mean sedentary minutes between married and not-married participants?

### **Q3 — Multiple Linear Regression**
How do age and marital status predict systolic blood pressure?

### **Q4 — Pearson Correlation**
Is weight correlated with sedentary minutes?

### **Q5 — Creative Analysis**
An additional inferential analysis using one of the following:
- Chi-square  
- T-test  
- ANOVA  
- Correlation  
(Selected automatically depending on variable availability.)

---

## Data Preparation Steps
- Loaded NHANES SAS `.xpt` files using `read_sas()`
- Merged datasets on participant ID (`SEQN`)
- Cleaned placeholder values (e.g., 77, 99, 7777, 9999)
- Recoded:
  - **Marital status** → married vs. not married  
  - **Education level** → bachelor’s degree or higher vs. less than bachelor’s
- Standardized key variables (e.g., systolic BP → `SYSBP`)

---

## Methods Used
- Chi-square test of independence  
- Independent samples t-test  
- Multiple linear regression  
- Pearson correlation  
- One-way ANOVA (if used in Q5)

---

## Results Summary
Each inferential test includes:
- Statistical test output (test statistic, p-value)
- Visualization (when appropriate)
- A short written interpretation in clear, plain language

These appear directly under the corresponding code cells within the notebook.

---

## Submission Information
This repository fulfills the assignment requirements for:

**HHA-507 — Inferential Analytics using NHANES (2021–2023 Cycle)**

The notebook is fully documented, includes all required analyses, and contains brief written summaries for each test.

---

