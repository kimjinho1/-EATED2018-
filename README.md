# -EATED2018-
## 주제: DQN을 이용한 고전게임 강화학습
### 인천대학교 전자공학과 김진호

__개발 환경: 아나콘다(jupyter notebook)__

#### references:

https://hunkim.github.io/ml/

https://tensorflowkorea.gitbooks.io/tensorflow-kr/content/g3doc/api_docs/python/constant_op.html

https://www.youtube.com/playlist?list=PLlMkM4tgfjnLSOjrEJN31gZATbcj_MpUm

http://ordo.tistory.com/68

#### Game environment: 

https://gym.openai.com/

http://solarisailab.com/archives/486

#### 1. 연구과정

![default](https://user-images.githubusercontent.com/29765855/48728221-b4009300-ec77-11e8-8e33-925c77718522.PNG)

방학 때 에디슨 프로그램을 하면서 딥러닝에 관심이 생겼고, 연구실 동료들과 파이썬을 공부했습니다.

개강 후에는 연구주제를 강화 학습으로 정했고 강화 학습 알고리즘을 공부한 후, 마지막으로 실제로 게임에 적용해보았습니다.

#### 2. DQN(Deep Q-Network)란?

![dqn](https://user-images.githubusercontent.com/29765855/48728606-badbd580-ec78-11e8-9758-feab716beaad.PNG)

#### 3. 적용한 게임들

![default](https://user-images.githubusercontent.com/29765855/48728804-5b31fa00-ec79-11e8-9dc4-8cef8d938c14.PNG)

1) Frozen Lake: S부터 G까지 H에 들어가지 않고 무사히 걸어가야 하는 게임

2) CartPole: 막대기를 넘어뜨리지 않게 하는 게임

3) CatchGame: 하늘에서 떨어지는 박스들을 잡는 게임

#### 4. 결과

##### 1) Frozne Lake

![lake](https://user-images.githubusercontent.com/29765855/48729123-2a05f980-ec7a-11e8-9fa8-1bcbcac826a5.PNG)

그래프를 통해 훈련 50번 이후부터는 S에서 G까지 계속 무사히 도착했다는 것을 확인할 수 있다.

오른쪽 그림은 모델의 정확도와, Q를 프린트 한 것이다. 

Q를 보면 16개의 행으로 되어있고 한 행안에 4개의 숫자가 있는데, 16은 State의 개수, 4는 Action(Left, down, right, up)을 의미한다.

##### 2) CartPole

![cartpole](https://user-images.githubusercontent.com/29765855/48966190-b6644380-f00f-11e8-8fc0-eef94ef23108.PNG)

훈련 회수에 따라 잘 학습된 것을 볼 수 있다.
(너무 오래 서있는 상황이 나와 훈련이 끝나지 않는 경우가 생겨서 최대 개수를 10000개로 제한을 했습니다)

##### 3) CatchGame

![catch](https://user-images.githubusercontent.com/29765855/48729509-1c9d3f00-ec7b-11e8-9265-6e0841905b62.PNG)

마찬가치로 학습이 잘 된 것을 볼 수 있다.

#### 5. 향후 연구

모델을 더 효과적으로 학습시키기 위해서 심층 신경망(DNN) 뿐만 아니라 CNN과 RNN 등을 공부!

다음 도전 과제: 슈퍼마리오!

![default](https://user-images.githubusercontent.com/29765855/48729758-bb29a000-ec7b-11e8-9baa-c5f3ee91d5a2.PNG)
