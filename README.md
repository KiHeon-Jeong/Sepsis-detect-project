# Sepsis-detect-project

MIMIC-IV 기반 패혈증/사망 예측을 위한 머신러닝 분석 저장소입니다.
이 저장소는 EDA와 모델링 자산만 포함합니다.

## 저장소 범위
- `EDA/`: 코호트 전처리, 탐색 분석, 결측치 처리, 중간 산출물
- `Modeling/`: 패혈증/사망 예측 모델 개발 노트북

## 폴더 구성
- `EDA/MIMIC-IV_ALL-PREPROCESS_1_Cohort_Data_EDA.ipynb`
- `EDA/MIMIC-IV_ALL-PREPROCESS_2_EDA.ipynb`
- `EDA/MIMIC-IV_ALL-PREPROCESS_3_missing_imputation.ipynb`
- `Modeling/MIMIC-IV_MODELING_1_DEATH_final.ipynb`
- `Modeling/MIMIC-IV_MODELING_2_SEPSIS_final.ipynb`
- `Modeling/Testing_otherhospitaldata_eICU_Demo.ipynb`

## 실행 환경
Python 3.10+ 권장

예시:
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install jupyter pandas numpy matplotlib seaborn scikit-learn lightgbm xgboost
jupyter lab
```

## 참고
- 웹 배포/연동 코드는 별도 웹서비스 저장소에서 관리합니다.
- `EDA/`의 CSV/DOCX 파일은 분석 과정 산출물입니다.
