# ML_algorithms
각종 기계학습, 회귀분석 등 예측모델링을 파이썬으로 구현

```
ANN : 인공신경망
decision_tree : 의사결정나무
non_ML/Regression : 회귀분석 및 가설검정
non_ML/non_linear_reg : 비선형 회귀(by gradient descent)
```

## ANN

> numpy를 이용해서 신경망 모델 구현

- 처음에는 수치해석 기법으로 parameters(W, b)를 최적화
- 이후 forward, backward 부분으로 나눠 backpropagation 구현
- 속도와 정확도 모두 backpropagation으로 구현한게 좋다.
- Activation function으로 처음에 sigmoid를 사용했는데 sample data(randomly selected)의 값이 너무 크거나 작은 경우 파라미터 적합이 제대로 진행되지 않아서 정규화를 할까하다가 그냥 relu 함수 사용.  



## Clustering

> K-means clustering 구현

**Process**

1. select k(the number of clusters)
2. select k center points randomly(or other proper methods)
3. for each x, select group(by nearest center, ucleadian distance)
4. update center points by each mean of group
5. repeat unitl not change group



## Decision Tree

> Decision tree 구현

**Process**

1. Finding column and row condition subject to minimize entropy(loss function)
2. Split data frame by condition
3. Repeat recursivly until can't reducing entropy or entropy=0

## Naive Bayes

> 나이브 베이즈 구현

설명변수가 조건부독입이라는 가정하에 베이지안 방법으로 예측



## Non_ML

### Regression

> OLS구현 및 검정 통계량 산출식 구현

### Non linear regression

> 비선형 회귀 구현(parameters optimize는 Gauss-newton method로)

