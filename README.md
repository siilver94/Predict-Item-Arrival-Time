# 물품 제시간 도착 여부 예측(Predict Item Arrival Time)

<br/>

<code><img height = "400"
src = https://github.com/siilver94/Predict-Item-Arrival-Time/assets/57824945/24f6ffe9-a25d-4fce-9faa-726affa4780e></code>

<br/>


## 프로젝트 소개

이 프로젝트는 고객 데이터를 활용하여 제품 배송 시간을 예측하여, `Reached on Time` 여부를 예측합니다.

<br/>

## 목표

- 제품 도착 시간 예측을 통한 물류 프로세스 최적화
- 머신러닝 모델을 활용한 정확한 `Reached on Time` 예측
  
<br/>


## 프로젝트 구조


**1. 데이터 수집**

- 국제 전자 상거래 회사의 고객 데이터베이스 확보
- **데이터셋:** 10,999 observations, 12 variables
  
**2. 데이터 전처리**

- 사용한 전처리 기술
  - OneHotEncoder, MinMaxScaler, OrdinalEncoder
- 결측치 및 이상치 처리
- 데이터 시각화를 통한 탐색적 데이터 분석
  
**3. 모델링**

- **사용한 머신러닝 알고리즘**
  - Logistic Regression
  - XGBoost
  - Random Forest
  - Logistic Regression with L1 and L2 Regularization
- 각 모델의 성능 평가를 위한 평가 지표: **Accuracy, ROC AUC**
  
**4. 시각화**

- **Seaborn**과 **Matplotlib**을 활용한 모델 성능 시각화


<br/>


### 데이터 Features

1. `ID`: 고객 식별 번호
2. `Warehouse block`: 회사의 대형 창고 블록 (A, B, C, D, E)
3. `Mode of shipment`: 제품 배송 방법 (Ship, Flight, Road)
4. `Customer care calls`: 배송에 대한 문의 전화 횟수
5. `Customer rating`: 고객 평가 (1부터 5까지)
6. `Cost of the product`: 제품 가격 (달러)
7. `Prior purchases`: 이전 구매 횟수
8. `Product importance`: 제품 중요도 (Low, Medium, High)
9. `Gender`: 성별 (Male, Female)
10. `Discount offered`: 제품 할인율
11. `Weight in gms`: 제품 무게 (그램)
12. `Reached on time`: 제품이 제시간에 도착했는지 여부 (Target 변수, 0 또는 1)

<br/>


## 사용기술

**언어:** Python

**라이브러리:** NumPy, Pandas, Scikit-learn

**시각화:** Seaborn, Matplotlib

<br/>



### 평가지표

- **Accuracy :** 모델의 전체 예측 정확도
- **ROC AUC :** 모델의 이진 분류 성능 측정
  
<br/>


## 리뷰

이 프로젝트를 통해 현실적이고 다양한 고객 데이터의 활용법을 배웠습니다. Logistic Regression, XGBoost, Random Forest 등 다양한 머신러닝 알고리즘을 적용하면서 각각의 특징과 장단점을 파악할 수 있었습니다. 또한, 모델링의 다양성을 경험하며 더 나은 선택을 할 수 있게 되었습니다.

Seaborn과 Matplotlib을 이용한 데이터 시각화는 데이터에 대한 통찰을 얻는 데 도움이 되었고 이를 통해 데이터를 그래프로 그리니 훨씬 이해하기 쉬웠습니다.

프로젝트를 진행하면서 데이터의 품질과 정확성이 얼마나 중요한지 깨달았고 좋은 데이터가 있어야 좋은 모델을 만들 수 있다는 것을 항상 느끼는 것 같습니다.

초기에는 데이터의 불일치와 결측치 처리에 어려움을 겪었지만,  전처리와 데이터 탐색을 통해 문제를 극복했습니다. 결국 데이터가 분석 가능한 형태로 변환되어 뿌듯했습니다.
어떤 머신러닝 알고리즘을 선택할지에 대한 고민이 있었지만, 여러 모델을 실험하고 비교하면서 각 모델의 특징을 이해하고 최종적으로는 가장 성능이 우수한 모델을 선택할 수 있게 되었습니다.
현재 모델들의 성능을 높이기 위해 파라미터 튜닝을 계획하고 있고. 더 나은 예측 결과를 위해 노력하고 공부가 필요해 보입니다.

이런 경험들을 바탕으로 다음 프로젝트에 더욱 더 나은 결과를 이끌어내고 싶습니다. 

