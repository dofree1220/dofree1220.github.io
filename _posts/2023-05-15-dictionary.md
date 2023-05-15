---
title: 사전
categories:
- python
- 2.프로그래밍과 데이터
tag: python
date: '2023-05-15 09:21:46'
---

# 사전

[→ 슬리드로 보기](https://app.slid.cc/docs/05616888c88e452cb740d48adc93976d)


---


목차

---

- 사전

- 사전 활용법

---


list를 사용하면 원하는대로 우리가 값을 지정하고 가져오려면 인덱싱을 이용해야하는 것도 배웠다.


이렇게 여러 값을 모아놓을 수 있는 자료형으로 python에서는 `사전 (dictionary)`라는 것이 존재한다.


보통 사전이 단어와 뜻이 쌍을 이루듯, python에서는 key와 value가 pair 쌍을 이룬다.


예시를 보자.

```Python
ex_dictionary = {
  5: 25, 
  2: 4,
  3: 9
}
```


값을 받아오려면 7번 줄 이후처럼 list는 index를 통해 받아왔지만, dictonary는 key값을 이용해 value를 받아온다.


위 코드를 기준으로 ex\_dictionary\[3\]이라면 그 키와 pair를 이루는 value가 ex\_dictionary\[3\]이 갖는 값이다.


새로운 쌍을 추가하려면 어떻게 해야할까 ?

```Python
ex_dictionary = {
  5: 25, 
  2: 4,
  3: 9
}

ex_dictionary[9] = 81

```


이렇게 사용하면 된다.


list와 dictionary의 차이점은 그럼 무엇일까 ?


list는 인덱스가 순서대로 진행되지만, dictionary는 딱히 순서란 개념이 없다.


list의 인덱스는 정수 값을 갖지만, dictionary는 정수일 필요 없이 문자열이여도 key가 될 수 있다.

---

### 사전 활용법

---


어떤 값들이 있는지 목록이 필요할 때 이 방법을 쓸 수 있


우리가 원하는 key, 또는 value 뒤에 keys(), value()라는 기능을 갖다 붙이면 key값, value값이 목록화 된다.


이것을 우리 입맛에 맞게 활용하면 된다.


items()라는 함수를 사용하 key, value 값을 둘 다 리턴하기 때문에 이를 평소 알아두면 좋다.

```Python
for key, value in ex_dictionary.items():
```
