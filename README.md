# Sepsis-detect-project

Machine learning workflow for sepsis and mortality prediction using MIMIC-IV based cohorts.
This repository contains EDA and modeling assets only.

## Repository Scope
- `EDA/`: preprocessing, cohort extraction analysis, missing-value handling, and intermediate datasets
- `Modeling/`: model development notebooks for sepsis and death prediction tasks

## Folder Structure
- `EDA/MIMIC-IV_ALL-PREPROCESS_1_Cohort_Data_EDA.ipynb`
- `EDA/MIMIC-IV_ALL-PREPROCESS_2_EDA.ipynb`
- `EDA/MIMIC-IV_ALL-PREPROCESS_3_missing_imputation.ipynb`
- `Modeling/MIMIC-IV_MODELING_1_DEATH_final.ipynb`
- `Modeling/MIMIC-IV_MODELING_2_SEPSIS_final.ipynb`
- `Modeling/Testing_otherhospitaldata_eICU_Demo.ipynb`

## Environment
Python 3.10+ is recommended.

Example setup:
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install jupyter pandas numpy matplotlib seaborn scikit-learn lightgbm xgboost
```

Run notebooks:
```bash
jupyter lab
```

## Notes
- This repo does not include web deployment code.
- CSV/DOCX files in `EDA/` are project artifacts used by notebooks.
