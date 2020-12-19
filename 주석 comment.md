# 주석 comment



cant use // and /**/



use # and """ """



```
#comment one
""""comment two"""
//error1
/*error2*/
```





## DocString

함수는 함수 내부에 주석을 쓴다.그래야 여러 부가기능이 가능하기 떄문!

```
def func1(param1):
	"""True return func
	
	args:
		param1 : ~~
		
	returns:
		bool : ~~
	"""
	return True
```



```
print(func1.__doc__)하면 저 주석문을 출력할 수 있따.
```

```
help(func1) 하면 저 주석문을 볼 수 있다.
```

