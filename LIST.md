# LIST



## PYTHON의 LIST?ARRAY?

첫 자료구조가 나올 떄 쯤

언제나 보던 array 대신에

뜬금없이 list가 나왔다.

c계열 언어만 쓰던 나로서는 혼동이 왔다 - 파이썬은 어레이를 리스트라고 부르나?아니면 어레이를 생략(?)하고 리스트를 가져다가 기본형으로 쓰나?





파이썬에도 어레이가 있기는 하지만, 기본적으로는 리스트를 쓴다.

리스트는 C의 어레이와는 다르고, 자바의 리스트와 오히려 비슷하다. 따라서 연속된 메모리에 있지 않다.다만 그점만 제외하면 임의접근등 어레이로 할 수 있는건 거의 다 가능함.그외 추가함수들도 보유.



파이썬의 리스트는 서로다른 타입의 데이터를 저장할 수 있다.좋은건지 나쁜건지..

리스트역시 리스트의 원소로 들어갈 수 있다.



리스트는 []를 통해 정의한다 

```python
l = [1,2,3]
//l[start:End:STEP]
```

# 리스트조작

```
s = [1,2,3,4]
s=[0:2] = [0,0]
// s = [0,0,3,4]
```

임의대입가능. 범위대입 가능

```
s[0:2] = []
// s=[3,4]
```

내용물 지우기

```
s.append(5)
//s = [1,2,3,4,5]
s.insert(0)
//s =[0,1,2,3,4]
n.pop()
//remove last and return it
n.pop(index)
//remove atIndex and return it
del n[0] 
//0번째 원소 삭제
del n
//n이라는 변수의 존재를 삭제(리스트없어짐)
n.remove(element)
//첫번째 element삭제
//없으면 error
```



## 리스트 결합

```
a = [1,2,3,4,5]
b= [6,7,8,9,10]
x= a+b
//x= 1~10
a=a+b //a+=b  , a.extend(b)
//a=1~10
```



## 메소드

```
r = [1,2,3,4,5,1,2,3]
r.index(3) //3의 인덱스인 2 리턴
r.index(3,4)//4번째 인덱스부터 검색한 3의 인덱스 인 7 출력
//index(value,start,end)
r.count(3)//3의 개수인 2 출력

5 in r //true 리턴

r.sort() // 정렬
r.sort(reverse = TRUE) //거꾸로 정렬
//sort(key,reverse)
r.reverse()//거꾸로만듬
```



## split 의 리턴 = 리스트

````
s = "hello world"
li = s.split(" ")
// li = [hello,world]
````



## 리스트 복사

대입으로는 얕은복사(주소복사)

copy()메소드를 통해 깊은복사

```
x= [ 1,2,3,4,5]
y = x //shallow
y = x.copy() //deep
y = x[:] //value cpy so deep
id()를 통해 가리키고 있는걸 알 수 있다
id(x)!=id(y) // in deep cpy
id(x)==id(y) // in shallow cpy
```

