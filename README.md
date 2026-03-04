# MIMIC Module (Sepsis & Mortality EDA/Modeling)

## 1) 개요
본 분석 코드들은 프로젝트 MIMIC(패혈증/사망 예측) 파트입니다.  
MIMIC-IV 기반 코호트 구성, 전처리/EDA, 결측 처리, 패혈증 및 사망 예측 모델링까지의 흐름으로 구성되어 있습니다.

## 2) 파일 구성
1. `EDA/MIMIC-IV_ALL-PREPROCESS_1_Cohort_Data_EDA.ipynb`  
   코호트 구성 및 기초 EDA
2. `EDA/MIMIC-IV_ALL-PREPROCESS_2_EDA.ipynb`  
   변수 중심 상세 EDA
3. `EDA/MIMIC-IV_ALL-PREPROCESS_3_missing_imputation.ipynb`  
   결측치 처리
4. `EDA/*.csv`  
   전처리/분석 중간 산출 데이터
5. `EDA/*SQL_Query*.docx`  
   코호트/변수 추출 SQL 기록 문서
6. `Modeling/MIMIC-IV_MODELING_1_DEATH_final.ipynb`  
   사망 예측 모델링
7. `Modeling/MIMIC-IV_MODELING_2_SEPSIS_final.ipynb`  
   패혈증 예측 모델링
8. `Modeling/Testing_otherhospitaldata_eICU_Demo.ipynb`  
   외부 데이터(eICU) 테스트

## 3) SQL/모델링 파이프라인 요약
- MIMIC-IV 기반 대상 환자 코호트 정의
- 시간 윈도우 기준 임상 변수 정리
- 결측/이상치 처리 및 학습셋 구성
- 패혈증/사망 예측 모델 학습 및 검증
- 필요 시 외부 데이터셋으로 성능 점검

## 4) 모델링 메모
- 본 저장소는 노트북 실험 로그 중심으로 구성됩니다.
- 웹서비스 API 연동용 모델 파일/코드는 웹서비스 저장소에서 관리합니다.

## 5) 수행 내용
- 임상 데이터 기반 위험 예측 파이프라인 설계
- 패혈증/사망 예측 모델 실험 및 비교
- 외부 데이터 기반 일반화 성능 검토

## 6) 기술 스택
- SQL (Oracle)
- Python
- MIMIC-IV
- Scikit-learn / LightGBM (실험 노트북 기반)

## 7) 참고
- 서비스 연동 구현은 `Sepsis-detect-project_Web-service` 저장소에서 관리합니다.
