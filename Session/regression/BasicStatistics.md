# Basic Statistics
1. Regression Problem
2. Classification Problem
## Cost Function
= Mean Squared Error
- Test data의 cost를 최소화하는 추정치를 찾아내는 것
- Bias : 예측값이 시제 값과 얼마나 다른가
- Variance : 예측값과 예측값의 평균의 차이의 제곱 기댓값
- 서로 반비례하는 성질이 있다
- MSE = bias^2 + Variance
- bias와 variance의 균형이 중요!
-----------------
- Continuous Varibale : 연속된 실수 값을 갖는 변수
- Categorical, Qualitative : 카테고리 값의 작은 숫자들
- Count variable : 음이아닌 정수값을 받는 변수
------------------------
## MLE 
- 다! 곱하는 거에욤
- 값들이 계속 곱해지면 어떤게 더 큰 값이냐? ㅋㅋ 이해 됬어용
- 다 곱하면 0으로 수혐해요! -> 비교가 안댑니다.
-> Log likelihood Function
# Linear Regression
## Estimating Parameter
### 단순회귀분석의 기본 가정(OLS 추정법 이용)
1. 회귀모형은 선형인 모형~
2. 오차항의 평균은 0, 분산은 델타^2
3.
4.
5.

- OLS : 최소자승법

~~ 왜 미분?


### Gradient Descent
- 문제점 : 복잡한 모델 사용 시 눈으로 판별하기 힘들다 ㅠㅠ, local minimum에 빠질 수 있슴

# Multiple Linear Regression
1. 추정치는 선형
2. 독립변수간 다중공선성은 없어야 한다
3. 자기상관이 없어야 한다
4. 등분산이어야 한다.
5. 잔차의 가정은 단순선형회귀와 동일

# Polinomial Regression
- 과적합이 일어나는 문제

## standart error, R square and t statistic
- Regression
- Error
- Total
 
 ### R-Squared
- *주어진 회귀식이 현상을얼마나 잘 설명하는가.
- 문제점
    - 많은 변수를 넣으면 상관있건없건 R^2값 ㅇㅣ증가한다.
    -
# Validation
## 다중공선성 문제점
1. 해가 무수히 많이 생김
2. 선대적으로 X'X의 역행렬이 없어서 값을 구할 수 없음
3. determinant 가 0에 수렴해 값을 구하기 히믇ㅁ
4. determinant 가 0에 수렴한다 : 표준편차를 높게 하고 t통계량의 p-value 값을 낮게 만든다.

### 진단법
1. corelation matrix를 그린다.
2. VIF 계수 확인

## 등분산성
분산이 일정해야 한다.

## Resampling Method
- Cross Validation
- The validation set Approach
    - 반 반~
- Leave One out Cross Validation
- <b>K fold Cross Validation <- 가장 많이 쓰인다.</b>

# Logistic Regression
- GLM 모델의 한 부류
- categorical , ordinal 한 변수에서 접근하기 조아염
- 분류 문제일 경우 관심 있는 종속변수를 $\pi$
## Binomail Response
### sigmoid Function
- 승산 : 임의의 사건 A가 발생하지 않을 확률 대비 일어날 확률의 비률
### cost Function


-------------------
로지스틱 Andrew ng 강의 듣기