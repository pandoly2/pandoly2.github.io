---
title: "Logistic Regression"
date: 2022-04-19T00:00:00+00:00
author: pandoly2
layout: post
permalink: /logistic-regression/
categories: Genel
tags: [pandoly2, machine learning, AI]
use_math: true
---

## 분류 (classification)
 - Training data 특성과 관계 등을 파악 한 후에, 미지의 입력 데이터에 대해서 결과가 어떤 종류의 값으로 분류 될 수 있는지를 예측하는것.
 예) 스팸문자 분류
 
![classification_image](/assets/images/blog_images/classification/classification.png){: width="100%" height="100%}
출처 : NeoWizard

 - 즉, Logistic Regression 알고리즘은, 
  1. Training data 특성과 분포를 나타내는 최적의 직선을 찾고(linear regression)
  2. 그 직선을 기준으로 데이터를 위(1) 또는 아래(0) 등으로 분류(Classification) 해주는 알고리즘

 - 이러한 Logistic Regression은 Classification 알고리즘 중에서도 정확도가 높은 알고리즘으로 알려져 있어서 Deep learning에서 기본 component로 사용되고 있다고함.

![classification_simple](/assets/images/blog_images/classification/classification_simple_flow.png){: width="100%" height="100%"}
출처 : NeoWizard
 - 출력 값 y가 0 또는 1 만을 가져야하는 분류 시스템에서, 분류 함수로 sigmoid함수를 사용하여 0/1 값을 갖게 할 수 있음
 - 즉, linear regression 출력 Wx + b 가 어떤 값을 갖더라도, 출력 함수로 sigmoid 를 사용해서
 1. sigmoid 계산 값이 0.5보다 크면 결과로 1이 나올 확률이 높다는 것이기 때문에 출력 값 y는 1을 정의
 2. sigmoid 계산 값이 0.5 미만이면 결과로 0 이 나올 확률이 높다는 것이므로 출력 값 y는 0을 정의
 - 0 또는 1을 분류하는 classification system 구현 할 수 있음.

 - Sigmoid 식 : 
 $$
y\ =\ sigmoid\left(z\right)\ =\ \phi \left(z\right)\ =\ \frac{1}{1\ +\ {e}^{-z}}
 $$

 ![classification_sigmoid](/assets/images/blog_images/classification/classification_sigmoid_graph.png)
 출처 : NeoWizard

 - 분류 시스템 최종 출력 값 y는 sigmoid 함수에 의해 논리적으로 1 또는 0 값을 가지기 때문에, 연속 값을 갖는 선형회귀 때와는 다른 손실함수 필요함.
 - 손실함수 (cross-entropy) 식 :    

$$
y\ =\ \frac{1}{1\ +\ {e}^{-1\left(Wx\ +b\right)}}\ ,\ t_i\ =\ 0\ or\ 1
$$
   
$$
 E\left(W,\ b\right)\ =\ -\ \sum _{i\ =\ 1}^n\left\{t_i\log {y_i\ }+\ \left(1-t_i\right)\log {\left(1\ -\ y_i\right)}\right\}
$$

 - classification 최종 출력 값 y 는 sigmoid 함수 에 의해 0 ~ 1 사이의 값을 갖는 확률적인 분류 모델이므로, 다음과 같이 확률변수 C 를 이용해 출력 값을 나타낼 수 있음.

**TBD: 이해하고 다시 작성**
 <font color=red>★ NeoWizard ppt 62page 참조</font> 

### logistic regression flow
![classification_flow](/assets/images/blog_images/classification/logistic_regression_flow.png)
















