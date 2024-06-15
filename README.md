# Fully Connected Neural Network

각 하나의 input layer, hidden layer, output layer로 구성된 fully connected neural network를 구성

## 프로젝트 구조
- `training.txt`: 학습 데이터셋 파일
- `test.txt`: 검증 데이터셋 파일

## 환경 및 라이브러리
- Python 3.x
- Numpy
- Matplotlib

## 사용 방법

### (a) 학습 및 검증 손실 플로팅

SGD 옵티마이저를 사용해 신경망 학습 후 epoch 당 평균 제곱 오차(MSE)에 대한 training&validaition loss 그래프로 시각화

1. `training.txt` 파일과 `test.txt` 파일에서 데이터 로드
2. 신경망 모델을 생성 및 학습
3. training loss와 validation loss 계산하여 저장
4. 각 epoch에서 raining loss와 validation loss 플롯팅

### (b) 은닉층 크기에 따른 학습 손실 비교

hidden layer의 크기를 2에서 16까지 변화시키면서 신경망을 학습 후 각 경우에 대한 training loss 비교

1. `training.txt` 파일에서 데이터 로드
2. hidden layer 크기에 따라 신경망 모델을 생성 및 학습
3. 각 hidden layer 크기에 대한 training loss 계산 후 저장
4. hidden layer 크기에 따른 training loss를 플롯

### (c) Adagrad 옵티마이저를 사용한 학습 손실 플로팅

SGD 대신 Adagrad 옵티마이저를 사용하여 신경망 학습 후 epoch 당 평균 제곱 오차(MSE)에 대한 학습 손실을 그래프로 시각화

1. `training.txt` 파일에서 데이터 로드
2. 신경망 모델을 생성하고 Adagrad 옵티마이저를 사용하여 학습
3. training loss 계산하여 저장
4. 각 epoch에서 training loss 플롯팅
