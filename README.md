# **📈Store Sales - Time Series Forecasting📉**
🔗 [Kaggle 대회 링크](https://www.kaggle.com/competitions/store-sales-time-series-forecasting)

## **0. 대회 소개**
- 시계열 예측을 사용하여 에콰도르 기반의 대형 식료품 소매업체인 Corporación Favorita의 매장 판매량(`sales`)을 예측하고자 함
  - Favorita 매장에서 판매되는 수천 개 제품들의 단위 판매량을 제품군 별로 정확하게 예측하는 모델을 구축하고자 함

## **1. 참여자**
|**팀원 1**|**팀원 2**|**팀원 3**|**팀원 4**|**팀원 5**|
|:----------:|:----------:|:----------:|:----------:|:----------:|
|<img src="" width = 100 height = 100>|<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/abe0ff1e-6df1-4863-bb9b-cd576aa7cc43" width = 100 height = 100>|<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/8fd038c6-3446-4e84-a593-a54f996ea427" width = 100 height = 100>|<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/b7c82bb7-1880-4f33-af22-c062f993f945" width = 100 height = 100>|<img src = "https://avatars.githubusercontent.com/u/98953721?v=4" width = 100 height = 100>|    
|[고도현](https://github.com/rhehgus02)|[박지현](https://github.com/Jihyun13579)|[서혜현](https://github.com/hyehyunseo)|[원서현](https://github.com/seohyun126)|[차수빈](https://github.com/chasubeen)|


## **2. 진행 과정**
- **기간**: 2023.1.01(월) ~ 2023.01.19(금)  
- **세부 일정**  
<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/0fc087b3-6e41-4d98-a8d9-d15cff380545" width = 500 height = 250>

- **역할**
  
|**이름**|**역할**|
|:-----:|:----------:|
|고도현|데이터 병합, 데이터 전처리, EDA - Type D, Modeling - Type D|
|박지현|데이터 병합, 데이터 전처리, EDA - Type A, Modeling - Type A|
|서혜현|데이터 병합, 데이터 전처리, EDA - Type C, Modeling - Type C|
|원서현|데이터 병합, 데이터 전처리, EDA - Type E, Modeling - Type E|
|차수빈|데이터 최종 병합, 데이터 최종 전처리, EDA - Type B, Modeling - Type B, 코드 최종 검토|

---
## **3. 과제 목표**
- 예측은 기상학뿐만 아니라 정부의 경제 성장, 과학적 미래 인구 예측뿐만 아니라 기업의 제품 수요 예측과 같은 다양한 분야에서 중요한 역할을 함
  - 특히 육상 식료품점에서는 정확한 재고 구매가 필요하며, 머신러닝을 통한 더 정확한 예측은 고객을 만족시키기 위해 필수적임
- 현재의 주관적인 소매 예측 방법은 데이터 부족으로 자동화하기 어려우며, 새로운 위치, 제품, 계절 변화, 예측할 수 없는 마케팅으로 인해 더욱 복잡함

> 여러 Favorita 상점에서 판매되는 수천 개의 품목에 대한 단위 판매를 더 정확하게 예측하는 모델 구축

### **📍 평가 지표**
- Root Mean Squared Logarithmic Error(`RMSLE`)
  - 다음과 같이 계산
- $$\sqrt{ \frac{1}{n} \sum_{i=1}^n \left(\log (1 + \hat{y}_i) - \log (1 + y_i)\right)^2}$$
  - $n$: 총 인스턴스 수  
  - $\hat{y}_i$: 인스턴스 $i$에 대한 타겟의 예측값  
  - $y_i$: 인스턴스 $i$에 대한 타겟의 실제값  

## **4. 디렉토리 구조**
```
Store-Sales-Forecasting
├─ 데이터 구조(정의).docx # ERD(Entity Relationship Diagram)
├─ 1. data_merging.ipynb # 데이터 병합
├─ 2. preprocessing.ipynb # 데이터 전처리
├─ 3. EDA_final.ipynb # EDA
├─ 4. Modeling_Final.ipynb # Modeling
│
├─1. merging # 데이터 병합
│  ├─고도현
│  │      데이터 병합_고도현.ipynb
│  │
│  ├─박지현
│  │      데이터_전처리_pdf파일.pdf
│  │      데이터_전처리_박지현.ipynb
│  │
│  └─원서현
│          1. data_merging.ipynb
│
├─2. preprocessing # 데이터 전처리
│      2. data_preprocessing(원서현).ipynb
│      2. preprocessing_차수빈.ipynb
│      kaggle_stocksales_전처리(서현).ipynb
│      kaggle_stocksales_전처리.ipynb
│      전처리_고도현.ipynb
│
├─3. eda
│      3. EDA_TypeA_박지현.ipynb
│      3. EDA_TypeB_차수빈.ipynb
│      3. EDA_TypeC_서혜현.ipynb
│      3. EDA_typeD_고도현.ipynb
│      3_EDA_typeE_원서현.ipynb
│
└─4. modeling
        4. Modeling_TypeA_박지현.ipynb
        4. Modeling_typeB_차수빈.ipynb
        4. Modeling_TypeC_서혜현.ipynb
        4. Modeling_TypeD_고도현.ipynb
        4_Modeling_TypeE_원서현.ipynb
```

## **5. Data Description**
**[🔗 데이터 병합](https://github.com/chasubeen/Store-Sales-Forecasting/blob/main/1.%20data_merging.ipynb)**  
**[🔗 데이터 전처리](https://github.com/chasubeen/Store-Sales-Forecasting/blob/main/2.%20preprocessing.ipynb)**  

- 일 단위 데이터
- 데이터 수집/가공 후 하나의 ```csv``` 파일로 가공
- 성격과 목적에 맞게 **5가지** 파일로 구분되어 있음

### **📌 ERD(Entity Relationship Diagram**
**[🔗 데이터 구조(정의)](https://github.com/chasubeen/Store-Sales-Forecasting/blob/main/%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EA%B5%AC%EC%A1%B0(%EC%A0%95%EC%9D%98).docx)**

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/15b8e943-95ff-42d2-a530-d6d84fb3f639" width = 700 height = 550>

### **1) train.csv**
- 학습용 데이터
- 데이터 건수: 300만개
- 데이터 시점: 2013-01-01 ~ 2017-08-15
- 중복 데이터: x

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/bbb6aad6-fb08-4b6e-b854-72ed97feda18" width = 700 height = 400>
  
### **2) stores.csv**
- 매장 메타데이터
- 데이터 건수: 54개
- 데이터 시점: x
- 중복 데이터: x

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/c57dad52-0127-4474-aeeb-8b66ff6f3bdd" width = 700 height = 300>
  
### **3) oil.csv**
- 일일 유가
- 데이터 건수: 1218개
- 데이터 시점: 2013-01-01 ~ 2017-08-31
- 중복 데이터: x

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/f7f759ed-36c5-40a5-9672-56cb89f079de" width = 700 height = 200>
  
### **4) transaction.csv**
- 거래 데이터, 하루 동안 매장에 방문한 사람 수 또는 하루에 생성된 송장(영수증) 수
- 데이터 건수: 83488개
- 데이터 시점: 2013-01-01 ~ 2017-08-15
- 중복 데이터: x

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/762079c9-66d5-4849-a2cc-145a8e1dc99c" width = 700 height = 250>

### **5) holidays_events.csv**
- 휴일 및 이벤트에 대한 메타 데이터
  - 공휴일의 규모가 가장 중요하다고 판단됨
    - 국가 공휴일인 경우 전 지역, 전 매장이 영향을 받음
    - 지역 공휴일인 경우 해당 지역(주, 도시)만 영향을 받음
- 데이터 건수: 350개
- 데이터 시점: 2012-03-02 ~ 2017-12-26
- 데이터 중복: O

<img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/2e672c47-45ec-485f-8d3d-c5d08600337c" width = 700 height = 450>

### **최종 train 데이터**

| Index | Column        | Description                     |
|-------|---------------|---------------------------------|
| 1     | id            | 각 데이터를 구분하기 위한 식별자|
| 2     | date          |판매일자                         |
| 3     | store_nbr     |매장 고유 식별번호               |
| 4     | family        |판매되는 제품군 유형             |
| 5     | sales         |매출액, **target 변수**        |
| 6     | onpromotion   |프로모션 대상 제품 수            |
| 7     | city          |도시                             |
| 8     | state         |주                               |
| 9     | type          |매장 유형                        |
| 10    | cluster       |유사한 매장들의 군집             |
| 11    | dcoilwtico    |유가(기름값)                     |
| 12    | transactions  |거래량                           |
| 13    | holiday       |공휴일 종류                      |

## **6. 시계열 분석**
- 시도표
- 시계열 분해(time series decomposition)
  - 추세(Trend): 우상향
  - 계절성(seasonality): 주로 연말(11~12dnjf)에 증가하고 연초(1~2월)에 감소하는 형태
  - 잔차 분석: 패턴이 나타나지 x
- 정상성
  - ACF, PACF
  - ADF 검정
---
- 데이터 파악 시 2가지 문제점을 파악
  - 매장마다 개업 일자가 다르다는 문제
  - 중간에 휴업을 한 경우들도 존재 -> 차분의 어려움

> 시간과 관련된 변수로 `year(연도)`, `quarter(분기)`, `month(월)`, `day_of_week(요일)` 변수 추가

## **7. EDA(데이터 탐색)**
- 5개의 파일을 병합/ 전처리 후 학습용 데이터에 대해 수행  
**[🔗 EDA](https://github.com/chasubeen/Store-Sales-Forecasting/blob/main/3.%20EDA_final.ipynb)**  

### **📌 type, cluster**
- `type`, `cluste`r에 따라 store은 어떻게 구분되는지 파악
  - `type`과 `cluster` 변수는 서로를 구분하는 데 중요한 역할을 하는 것으로 확인됨
- 또한, 가게의 type마다 매출액의 크기와 분포에 큰 차이가 있음을 확인
  <img src = "https://github.com/chasubeen/Store-Sales-Forecasting/assets/98953721/90aec38d-746f-476e-9fa0-a2bc346ef595" width = 700 height = 500>

> type에 따라 각각 다른 예측 모델을 개발하기로 결정

- 이후 각 type별로 EDA를 진행한 후 이상치 제거, 최종적으로 모델링에 활용할 변수 선택

| Type |최종 활용 변수                   |
|-------|---------------------------------|
| A     |`store_nbr`, `family`, `onpromotion`, `state`, `cluster`, `dcoilwtico`, `holiday`, `year`, `quarter`, `month`, `day_of_week`|
| B    |`store_nbr`, `family`, `onpromotion`, `city`, `cluster`, `dcoilwtico`, `holiday`, `year`, `quarter`, `month`, `day_of_week`|
| C    |`store_nbr`, `family`, `onpromotion`, `state`, `cluster`, `dcoilwtico`, `holiday`, `year`, `quarter`, `month`, `day_of_week`|
| D     |`store_nbr`, `family`, `onpromotion`, `city`, `cluster`, `dcoilwtico`, `holiday`, `year`, `quarter`, `month`, `day_of_week`|
| E     |`store_nbr`, `family`, `onpromotion`, `dcoilwtico`, `holiday`, `year`, `quarter`, `month`, `day_of_week`|

## **8. 모델링(회귀 분석)**
- `RandomForestRegressor` 활용
- `HyperOpt`를 활용한 하이퍼 파라미터 튜닝

**[🔗 Modeling](https://github.com/chasubeen/Store-Sales-Forecasting/blob/main/4.%20Modeling_Final.ipynb)**  

| Type |RMSE|
|-------|------|
|A|0.323|
|B|0.371|
|C|0.378|
|D|0.355|
|E|0.139|

## **9. 예측 & 결과 정리**
- test 데이터를 `type`별로 분리 후 각 모델을 활용하여 예측 수행
  - 예측 이후 해당 매장에서 판매하지 않는 제품군의 경우 `sales`를 0으로 수정
- 대부분 `onpromotion`과 제품군(`family_`)의 종류가 모델의 예측 성능에 큰 영향을 미침
- 최종 LeaderBoard RMSLE: **0.54718**

---
## **회고**

### **차수빈**
- 이후 BDA 공모전과 비슷한 환경에서 실습을 하기 위해 `RandomForestRegressor`만 사용하였는데, 범주형 변수가 많은 상황에서 해당 모델은 다른 RNN 기반 모델이나 ARIMA 등의 통계적 모형에 비해 예측 성능이 떨어지는 것 같다.
- 데이터 이해에 많은 시간을 허비하여 모델링에 더 많은 노력을 기울이지 못해 아쉽다.
