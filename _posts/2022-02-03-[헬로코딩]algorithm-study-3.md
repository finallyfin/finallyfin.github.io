---
layout: post
title: [헬로코딩] algorithm study-3
categories: algorithm
author: "Jiyoung Cheon"
meta: ""
tags: [algorithm, study, 헬로코딩]
---

#### 재귀 함수에서 호출스택 사용

  먼저 팩토리얼 함수가 어떻게 동작 하는지 살펴보자. factorial(5)는 5!라는 뜻이고 이는 5*4*3*2*1로 정의되는 값이다. 재귀 함수를 사용해서 팩토리얼이 어떻게 계산 되는지 알아보자.

  ```python
  def fact(x):
    if x == 1:
      return 1
    else:
      return x * fact(x-1)
  ```
스택을 사용하면 확인해야 할 상자 더미를 일일이 추적하지 않아도 되므로 편리하다. 하지만 모든 정보를 저장해야 하므로 메모리를 많이 소비한다.

* 모든 함수 호출은 호출 스택을 사용한다.
* 호출 스택은 너무 커져서 메모리를 엄청나게 소비할 수도 있다.
