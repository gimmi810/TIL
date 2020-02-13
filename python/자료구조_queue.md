자료구조
===================================
> 시연사이트 : https://visualgo.net/en/list

## Queue
* FIFO (First-In, First-Out)
* 멀티 태스킹을 위한 프로세스 스케쥴링 방식을 구현하기 위해 많이 사용
  * enqueue : 큐에 데이터를 넣는 기능
  * dequeue : 큐에서 데이터를 꺼내는 기능
```
queue_list = list()
def enqueue(data):
    queue_list.append(data)
def dequeue():
    data = queue_list[0]
    del queue_list[0]
    return data
```
```
for index in range(10):
    enqueue(index)
len(queue_list)
// 10
dequeue()
// 0
```

## LifoQueue
| LIFO(Last-In, First-Out)

## PriorityQueue
| 우선순위
```
data_queue.put((10, "korea"))
data_queue.put((5, 1))
data_queue.put((15, "china"))
data_queue.get()
// (5, 1)
```
