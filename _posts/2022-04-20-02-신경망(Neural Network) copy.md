---
title: "신경망 (Neural Network)"
date: 2022-04-20T00:00:00+00:00
author: pandoly2
layout: post
permalink: /neural-network/
categories: Genel
tags: [pandoly2, machine learning, AI]
use_math: true
---

### 신경망의 구조
- 퍼셉트론이 여러층 연결되어 구성되듯이 인간의 신경계도 여러개의 뉴런의 신호전달로 이루어진다. 
- 인공신경망도 신경계와같이 여러개의 노드들간의 입력신호와 출력신호, 가중치, 바이어스에따라서 신호 전달이 이루어진다.   
**※ 인공 신경망과 퍼셉트론으 가장 큰 차이는, 퍼셉트론은 가중치를 결정할때 사람이 직접 관여를 해야하지만, 인공 신경망은 데이터를 통해 스스로 학습하여 가중치를 결정한다는 점이다.**

- 다층 퍼셉트론   
![perceptron_xor_detail_solution](/assets/images/blog_images/Perceptron/perceptron_xor_detail_solution.png)

- 신경망   
![nn_natural](/assets/images/blog_images/NeuralNetwork/nn_natural.png)

- 인공 신경망의 구조   
![nn_artificial](/assets/images/blog_images/NeuralNetwork/nn_artificial.png)
- 인공 신경망은 입력층, 은닉층, 출력층으로 구성된다. 
- 각각의 원은 뉴런 또는 노드라는 용어로 사용된다
 
### 인공 신경망 구성
 - 퍼셉트론의 flow를 생각해보면, linear regression의 출력값을 classification 함수를 사용하여 분류를 했다. 
 - 신경망의 뉴런또한 어떠한 신호가 들어왔을때, 특정한 임계치를 넘지않으면 그다음 뉴런으로 신호가 발생 되지않는다. 
 - 이것과 마찬가지로 인공 신경망에서도 **활성화 함수**라고 명칭하는 분류기 혹은 해당신호를 다음 노드의 입력으로 출력할 지를 결정하는 함수가 존재한다. 
 - 그림은 다음과 같다. 

![nn_activation_struct](/assets/images/blog_images/NeuralNetwork/nn_activation_struct.png)
출처 : 밑바닥부터 시작하는 딥러닝

 - 입력신호와 가중치 그리고 바이어스를 조합한 결과가 a노드가 되고 a노드는 h()라는 활성화 함수를 통과하여 y노드로 변환된다.
 - 즉 활성화 함수를 통해 신호가 1/0으로 구분된다.

### 활성화 함수의 종류
 - Sigmoid
 - ReLU
 - Leaky ReLU
 - tanh   
 - 활성화 함수에대해서 좀더 자세히 알고싶다면 다음 블로그를 참고하면 된다.  [활성화 함수 종류](https://wooono.tistory.com/209)










