# <a href=https://arxiv.org/abs/1706.03762>Attention Is All you need</a>
## Abstract
* Transformer라는 새로운 network architecture
* 신경망을 사용하지 않음
* 불필요한 recurrence나 convolution을 제거한
* Attention Machanism에반 기반하고 있다
* **병렬 처리가 가능**
* **훈련 시간이 덜 걸린다**

## Introduction
* 순환적 모델은 병렬 처리가 불가능하다
* Attention은 거리에 관계없이 dependency를 모델링 할 수 있다.
* Transformer 쓰면 병렬 처리하면서도 global dependency를 가져올 수 있다.


## Multi Head Attention
- dot product attention 구조가 중첩된 형태
- scaled dot product
  - query : 찾고자 하는 단어
  - key : 사전에 등록된 단어
  - value : key에 해당하는 의미
  - 과정
    1. Q, K 에 대한 어텐션 스코어 맵을 만든다
    2. 스케일 조정을 한다
    3. 선택적으로 마스크를 적용한다
    4. 소프트맥스 함수를 적용한다.
    5. value 에 대해 가중합을 구한다
  - self attention은 query 행렬과 key 행렬이 전치관계
- 순방향 어텐션 마스크
  - 디코더 파트에서 자신보다 뒤에 있는 단어를 참고하지 않게 하는 기법

## Position wise feed foward network
- 