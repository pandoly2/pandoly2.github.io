---
title: "수학개념 (Prerequisite for Machine Learning)"
date: 2022-04-18T00:00:00+00:00
author: pandoly2
layout: post
permalink: /Prerequisite-of-Math/
categories: Genel
tags: [pandoly2, machine learning, AI, Math]
use_math: true
---

## 수치미분   

### 미분으로 얻을 수 있는 Insight
 -> 입력 변수 x가 미세하게 변할때, 함수 f(x)가 얼마나 변하는지 알 수 있는 식을 구해라.   
 -> 한수 f(x)는 입력 x의 미세한 변화에 얼마나 민감하게 반응하는지 알 수 있는 식을 구해라.        
**Insight**   
 -> 입력 x 를 현재 값에서 아주 조금 변화시키면, 함수 f(x)는 얼마나 변하는가?   
 -> 함수 f(x)는 입력 x의 미세한 변화에 얼마나 민감하게 반응하는가?   

<font color=red> 어떤 값 x가 아주조금 변할때 y값의 미세한 변화량을 나타내는 기울기 혹은 크기 </font>

### 기본 미분 공식
$$
f'\left(x\right)\ =\ \frac{df\left(x\right)}{dx}\ =\lim _{\Delta x \to 0}{\frac{f\left(\left(x\ +\ \Delta x\right)\ -\ f\left(x\right)\right)}{\Delta x}}
$$
   
### 중앙차미분
$$
f'\left(x\right)\ =\ \frac{df\left(x\right)}{dx}\ =\lim _{\Delta x\to 0}^{ }\frac{f\left(\left(x\ +\ \Delta x\right)\ -\ f\left(x\ -\ \Delta x\right)\right)}{2\Delta x}
$$

![Numerical_Differentiation](/assets/images/blog_images/NumericalDifferentiation/Numerical_Differentiation.jpg "Numerical Differentiation"){: width="100%" height="100%"}




참조 : [https://blog.naver.com/PostView.naver?blogId=mykepzzang](https://blog.naver.com/PostView.naver?blogId=mykepzzang&logNo=220072089756&parentCategoryNo=&categoryNo=16&viewDate=&isShowPopularPosts=false&from=postView)

### 편미분

예 ) $$ f\left(x,\ y\right)\ =\ 2x\ +\ 3xy\ +\ y3 $$ 에 대해,

1. 변수 x에 대하여 편미분   
$$
\frac{\partial f\left(x,y\right)}{\partial x}\ =\ \frac{\partial \left(2x\ +\ 3xy\ +{y}^3\right)}{\partial x}\ =\ 2\ +\ 3y
$$

2. 변수 y에 대하여 편미분   
$$
\frac{\partial f\left(x,y\right)}{\partial x}\ =\ \frac{\partial \left(2x\ +\ 3xy\ +{y}^3\right)}{\partial x}\ =\ 3x\ +\ 3y^2
$$
   
### Chain Rule
합성함수란 여러 함수로 구성된 함수로서, 이러한 합성함수를 미분하려면 '합성함수를 구성하는 각 함수의 미분의 곱'으로 나타내는 chain rule(연쇄 법칙) 이용
Ref. NeoWizard PPT 5 page (개인용)


