# Sepsis-detect-project

MIMIC-IV 기반 패혈증/사망 예측 모델 개발 저장소입니다.

## 개요
응급실 환자 코호트를 기반으로 전처리, EDA, 모델링을 수행한 산출물을 관리합니다.

## 디렉터리
- `EDA/`: 코호트 추출 검토, 결측치 처리, 분석 산출물
- `Modeling/`: 패혈증 및 사망 예측 모델 실험

## 포함 자산
- 전처리/EDA 노트북
- 사망 예측/패혈증 예측 모델링 노트북
- 외부 데이터(eICU) 테스트 노트북

## 실행 방법
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install jupyter pandas numpy matplotlib seaborn scikit-learn lightgbm xgboost
jupyter lab
```

## 비고
웹 애플리케이션 실행 코드는 별도 웹서비스 저장소에 있습니다.
