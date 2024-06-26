### 문제

우주선이 모든 행성을 방문하기 위해서는 **어떤 행성부터 방문할지 결정**하고자합니다.
우주에 있는 오브젝트들의 거리는 **현재 우주선에서 왼쪽에 있으면 음수**로, **오른쪽에 있으면 양수**로 표기됩니다.

즉, 다음과 같은 상황이라고 가정해봅니다.

🌌🪐✨✨🚀✨🌌✨✨🪐

이때 우주선의 왼쪽에 있는 행성은 우주선으로부터 -3의 위치, 오른쪽에 있는 행성은 우주선으로부터 5의 위치에 있습니다.

이제 행성 중 **가장 가까운 세 곳**에 방문하고자 하는 우주선이 어떤 행성에 방문해야하는지 결정하는 프로그램을 완성해주세요.

### 입력

입력은 다음과 같이 배열 내 딕셔너리 형태로 오브젝트의 타입인 **type** 및 우주선으로부터 거리인 **dist**로 입력됩니다.

```python
[
	{"type": "planet", "dist": 10},
	{"type": "star", "dist": -3},
	{"type": "milkyway", "dist": 2},
	{"type": "planet", "dist": 5},
	{"type": "planet", "dist": -7},
	{"type": "star", "dist": 4},
	{"type": "planet", "dist": 6},
	{"type": "planet", "dist": -1},
	{"type": "star", "dist": 8},
	{"type": "milkyway", "dist": -9}
]
```

### 출력

```python
[-1, 5, 6]
```

### 샘플 코드

```python
def solution(arr):
  # 코드 작성
  return arr

arr = [
  {"type": "planet", "dist": 10},
  {"type": "star", "dist": -3},
  {"type": "milkyway", "dist": 2},
  {"type": "planet", "dist": 5},
  {"type": "planet", "dist": -7},
  {"type": "star", "dist": 4},
  {"type": "planet", "dist": 6},
  {"type": "planet", "dist": -1},
  {"type": "star", "dist": 8},
  {"type": "milkyway", "dist": -9}
]

print(solution(arr))
```
