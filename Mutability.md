# Mutable Object
##### Mutable object는 객체 생성 후 값을 변경할 수 있다.<br>
예) list, bytearray, array.array, collections.deque and memoryview
```PYTHON
>>> x = 1
>>> y = x
>>> y += 3
>>> x
1
>>> y
4
```
# Immutable Object
##### Immutable object는 객체 생성 후 값을 변경할 수 없다.<br>
예) number, tuple, str and bytes
```PYTHON
>>> x = [1,2]
>>> y = x
>>> y.append(3)
>>> x
[1,2]
>>> y
[1,2,3]
```
# Call by value
##### string이나 tuple같은 immutable 변수를 함수에 넘겨줄때, call by value가 일어난다. 변수의 주소가 함수의 인자로 들어가지만, immutable 변수이기 때문에 값의 변화를 줄 수 없다.

# Call by reference
##### list같은 mutable 변수를 함수에 넘겨줄때, call by reference가 일어난다. 변수의 주소가 함수의 인자로 들어가 값을 바꿔준다.

# immutable vs mutable
```PYTHON
def is_ mutable(arg1, arg2) :
	print(“a의 주소는 %d, b의 주소는 %d”%(id(arg1),id(arg2)))
	if(id(arg1)==id(arg2)) :
		print(type(arg1),”is mutable”)
	else:
		print(type(arg1),”is immutable)
	pass
```
