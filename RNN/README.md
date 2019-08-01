# RNN

**RNN(Recurrent Neural Network)** : 순환 신경망인 RNN은 상태가 고정된 데이터를 처리하는 다른 신경망과는 달리 **자연어 처리나 음성 인식처럼** 순서가 있는 데이터를 처리하는데 강점을 가진 신경망이다.

* **자연어** : 사람들이 일상적으로 쓰는 언어



# 1. MNIST를 RNN으로

우선 개념을 쉽게 이해하기 위해, 자연어가 아닌 이전에 사용했던 MNIST를 이용해 보자.

* **RNN 기본 개념**

  <img src="https://sunghan-kim.github.io/assets/images/book/3minDL/ch10-02-rnn-basic-concept.jpg">

  > **셀(Cell)** : 한 덩어리의 신경망

  * RNN은 이 셀을 여러 개 중첩하여 심층 신경망을 만든다. 
  * 이런 구조로 인해 학습 데이터를 단계별로 구분하여 입력해야 한다.



* **MNIST를 RNN 방식으로 학습시키는 방법**

  <img src="https://sunghan-kim.github.io/assets/images/book/3minDL/ch10-03-mnist-data-for-rnn.jpg">

  * MNIST 데이터가 가로, 세로 28 X 28 크기이므로 가로 한줄의 28픽셀을 한 단계의 입력값으로 삼고 28단계를 거쳐 데이터를 입력받는 개념이다.



<img src="https://image.slidesharecdn.com/class3-170731055010/95/rnn-mnist-image-7-1024.jpg?cb=1501480262">

> 1번째 계층의 출력으로는 2번째 계층이 나와야하고,
>
> 2번째 계층의 출력으로는 3번째 계층이 나와야함을 학습시킨다.

