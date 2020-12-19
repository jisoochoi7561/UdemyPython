# enumerate



```
for i in [a,b,c]:
	print(i)
```

를 하면

a b c가 나온다

파이썬의 for문은 인덱스 정보를 포함하지 않는다.

따라서 인덱스정보를 얻기위해 enumerate를 쓴다.

```
for i,c in enumerate([a,b,c]):
	print(i,c)
```

를 하면

0 a 

1 b

2 c

가 나온다.