# ABC Bank customer churn rate analysis

## 개요 및 문제 설정

---

금융회사 특히 이번 주제인 은행에서 고객의 이탈을 방지하는 것은 매우 중요하다.

고객 이탈을 줄여야 하는 주된 이유는 다음과 같다.

은행은 고객이 예치한 돈으로 다른 개인고객 혹은 기업고객에게 대출을 해주면서 대출이자를 받는 예대마진의 수익구조를 기반으로 한다.
예대마진의 수익 이외로 은행 자체에서 재투자를 하여 비이자수익을 얻는다.
따라서 은행에 예치를 하는 고객을 최대한으로 유치해야하며 기존의 고객들이 이탈하는 것을 방지하여야 한다.
고객 이탈 방지가 중요한 또 다른 이유는 대부분의 사람들은 자산은 금융회사에 예치를 하기 때문에 회사에서 고객이 이탈하는 것은 다른 회사로 그 고객이 유입되는 것이기 때문에 산업 내 경쟁력을 높이는 측면에서도 의미를 가질 수 있다.
본 프로젝트에는 ABC Bank의 고객 이탈 데이터를 머신러닝 알고리즘으로 분석하는 것을 목적으로 한다.

## 과정

---

- 데이터 EDA
  - 이진 분류 특성 별 고객 이탈 현황
  - 특성 간 상관관계 도출
- 분류모델 설정
  - AUC Score 기준으로 결과 도출
  - LOGISTIC, RANDOM FOREST, XGBOOST 모델 진행 후 XGBOOST 선정
- 특성중요도
  - PERMUTATION INPORTANCE로 주요 특성 도출
  
## 해석 및 결과

---

- 상품, 나이, 정회원 유무 별로 이탈율 추이 확인
  - 1, 2 상품은 인기와 유지비율이준수 3, 4 상품은 가입률이 적고 이탈고객이 유지비율 보다 높으므로 고객만족도가 낮음
  - 3, 4 상품 폐기 -> 유지비 절약
  - 3, 4 상품의 가입 고객의 나이가 4,50대 중장년층 -> 중장년층 대상의 새로운 상품개발이 필요
  - 고객의 정회원 가입을 유도할 필요
- 중장년층 모바일 금융 지원
  - 50대 이상 고객의 모바일 금융 사용↑
  - 금융 정보를 모바일로 획득3, 4 보완 상품 개발50대 이상, 정회원이 아닌 고객에게앱 알림을 통해 정회원 가입 시 혜택이 주어지는 새로운 상품 알림 발송
