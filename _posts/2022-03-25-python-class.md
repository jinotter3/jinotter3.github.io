---
layout: post
title: Python class(파이썬 클래스)
subtitle: class
categories: Python
tags: [Python, ML]
--- 
# 파이썬 클래스

파이썬 클래스를 공부하면서 알게된 내용들을 정리해보려고 한다. 

## Constructor vs Destructor
### Constructor __init__
파이썬의 `__init__()` 함수는 class의 object가 instantiated 되자마자 실행된다.    
```python 
class Person:
    def __init__(self, name):
        self.name = name
        print(self.name)

otter = Person('Jin Otter')
```

- 실행결과     

```
Jin Otter
```

### Destructor __del__
파이썬의 `__del__()` 함수는 **Python Garbage Collector**와 작동한다.    
Python에서 생성되는 모든 Object는 Object가 참조되는 수인 reference count를 가지고 있다. Python의 `sys.getrefcount(object)`는 object의 참조 갯수(reference count)를 알려주는 함수로 작동한다. 
```python
import sys 
sys.getrefcount(3)
```
- 실행결과

```idle
694
# 시스템에 따라서 3이 사용되는 숫자도 변한다. 
# 필자는 머신러닝 라이브러리가 설치된 환경에서 실행하여 숫자가 크게 나온 듯 하다. 
```
<br>
이후, a = 3, b = 3과 같이 3을 가리키는 변수를 늘리면 참조의 개수가 증가한다. 
```python
import sys
a = 3 
sys.getrefcount(3)
```
- 실행결과

```idle
695
```

<br>
이후 `del a`등을 통해 3을 가리키는 변수가 줄어들면 참조 개수가 감소하는 모습을 볼 수 있다. 이 때 참조 개수가 0이 되는 순간, 3이라는 객체는 자동으로 Garbage collector에 의해 소멸한다. 
