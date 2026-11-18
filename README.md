# Titanic Feature Engineering

Titanic 생존 예측(분류)을 대상으로 결측치 처리, 인코딩, 스케일링, 파생변수, 변수 선택에 따른 성능 차이를 비교한 프로젝트입니다.

## 데이터
- Kaggle: Titanic - Machine Learning from Disaster (`train.csv`, 891행 × 12열)
- https://www.kaggle.com/competitions/titanic/data

## 폴더 구조
- `data/` 원본 데이터
- `notebooks/titanic_fe.ipynb` 전체 분석 노트북
- `figures/` 저장된 그래프
- `results/` 실험 결과표(CSV)
- `report/` 제출용 PDF

## 실행 방법
1. `python -m venv .venv` 후 가상환경 활성화
2. `pip install -r requirements.txt`
3. `notebooks/titanic_fe.ipynb`를 위에서부터 순서대로 실행 (`random_state=42` 고정)

## 구성
EDA → 파생변수 → 전처리 비교 실험(Base, Exp-1~3) → 추가 통제 실험 → 변수 선택 → 모델 비교 → GridSearchCV · SHAP · AutoML → 결론