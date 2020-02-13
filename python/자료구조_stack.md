자료구조
===================================
> 시연사이트 : https://visualgo.net/en/list

## Stack
* LIFO (Last In, Fisrt Out)
* 스택은 단순하고 빠른 성능을 위해 사용
* 보통 배열 구조를 활용해서 구현하는 것이 일반적
  * 단점 : 저장공간 낭비
* 파이썬의 경우 재귀 함수는 1000번까지만 호출이 가능


```
# 재귀 함수
def recursive(data):
    if data < 0:
        print ("ended")
    else:
        print(data)
        recursive(data - 1)
        print("returned", data)
```
```
recursive(4)
// 결과
4
3
2
1
0
ended
returned 0
returned 1
returned 2
returned 3
returned 4
```

| push, pop 구현
```
stack_list = list()
def push(data):
    stack_list.append(data)
def pop():
    data = stack_list[-1]
    del stack_list[-1]
    return data
```
```
for index in range(10):
    push(index)
pop()
// 9
```
