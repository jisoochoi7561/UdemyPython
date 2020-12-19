# Zip

```
days = ['mon','tue','wed']
fruits = ['apple','banana','orange']
drinks = ['coffee','tea','beer']
```

mon - apple - coffee 의 조합으로 3줄을 출력하려면



```
for i in range(len(days)):
	print(days[i],fruits[i],drinks[i])
```

를 해야한다.



zip을 써서 대체가능하다.

```
for day,fruit,drink in zip(days,fruits,drinks):
	print(day,fruit,drink)
```



zip의 반환은 리스트들의 리스트이다.