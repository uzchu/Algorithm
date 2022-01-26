## DFS&BFS



## DFS(깊이우선탐색)

- 현재 정점에서 갈 수 있는 점들까지 들어가면서 탐색
- 스택 또는 재귀함수로 구현

#### stack

```python
stact = []

stack.append(n)
stack.pop(n)
```

- LiFo

#### 재귀함수

```python
def recursive_function():
    #종료조건 명시
    if i ==100:
        return
	print(i, '번째 재귀 함수에서', i+1, '번째를 재귀함수를 호출합니다')
	recursive_function(i+1)
    print(i,'번째 재귀함수를 종료합니다')
	
recursive_function(1)
```

- 재귀함수를 사용할 때는 재귀함수의 종료조건을 명시해야 함





## BFS(너비우선탐색)

- 현재 정점에서 연결된 가까운 점들부터 탐색
- 큐를 이용해서 구현

#### Queue

```python
from collections import deque

queue = deque()

queue.append(n)
queue.popleft(n)
```

* FiFo
* 파이썬에서 리스트 자료형으로 큐를 구현할 수 있지만, 시간복잡도가 높아서 비효율적으로 계산될 수 있어 deque 이용하는 것이 좋음

- 먼저 들어온 순서대로 출력하려면 queue를 역순으로 출력

