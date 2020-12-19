# DIctionary

```
d = {"key1" : value1,"key2":value2}//생성
//d = {"key1" = value1,"key2"=value2}//생성
//d = ([("key1",value1)("key2",value2)]) //두개짜리 튜플들의 리스트를 넣어줘도 생성됨
d["key1"]//value1리턴
d["key1"] = value3 //수정
//value와 key들은 파이썬이 늘 그랬듯 타입들이 다를 수 있다!!(개꿀)
```



## methods

```
d={'x' : 10,'y':20}
d.keys() //return key list
d.values() //return value list
d['x']//return 10
d.get(x)// return 10

d['z'] //error
d.get('z') // NoneType

d2 = {'x':100,'j':500}
d.update(d2) // x = 100 y = 20 j = 500

d.pop('x') // return 100 and remove key x 
del d['y'] // remove key y
d.clear() // d is empty dictionary
'a' in d // true if key a is in d

```



## copy

list 처럼 deepcopy를 하려면 copy()메소드 사용