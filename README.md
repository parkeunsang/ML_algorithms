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