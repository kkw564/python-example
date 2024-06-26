### 문제

숫자 야구는 플레이어가 상대방이 생각하고 있는 숫자의 조합을 맞추는 게임입니다. 이 게임에서는 컴퓨터가 0부터 9까지의 숫자 중 서로 다른 3개의 숫자를 랜덤으로 선택합니다. 플레이어는 이 3개의 숫자를 정확한 순서로 맞추어야 합니다.

### 게임 규칙

1.  컴퓨터는 0에서 9 사이의 서로 다른 숫자 3개를 랜덤하게 선택합니다.
2.  플레이어는 컴퓨터가 선택한 숫자 3개의 값을 그리고 그 순서를 맞추어야 합니다.
3.  플레이어가 숫자를 입력할 때, 컴퓨터는 결과를 "스트라이크"와 "볼"로 알려줍니다.
    - **스트라이크**: 숫자의 값과 위치가 모두 맞을 때
    - **볼**: 숫자의 값은 맞지만 위치가 틀렸을 때
4.  플레이어가 모든 숫자의 값을 그리고 순서를 정확히 맞추면 게임이 종료됩니다.

### 요구사항

숫자 야구 게임을 파이썬으로 구현할 때, 다음 요구 사항들을 맞춰 프로그램을 작성하세요.

1.  컴퓨터가 0에서 9 사이의 서로 다른 숫자 3개를 랜덤으로 선택하게 합니다.
2.  사용자로부터 3개의 숫자를 입력받되, 각 숫자는 0에서 9 사이여야 하며, 서로 달라야 합니다.
3.  사용자가 입력한 숫자와 컴퓨터가 선택한 숫자를 비교하여 스트라이크와 볼의 수를 알려줍니다.
4.  사용자가 컴퓨터의 숫자를 모두 맞출 때까지 2-3번 과정을 반복합니다.
5.  게임이 끝나면 사용자가 몇 번 만에 숫자를 모두 맞췄는지 알려줍니다.

### 추가사항

1. 같은 수를 입력 받으면 "중복되는 숫자입니다. 다시 입력하세요." 를 출력합니다.
2. 입력 받는 숫자가 1 ~ 9사이 값이 아니면 "범위를 벗어나는 숫자입니다. 다시 입력하세요."를 출력합니다.

### 샘플 코드

```python
from random import randint

def generate_answer():
    answer = []

    # 코드 작성

    print("1과 9 사이의 서로 다른 숫자 3개를 랜덤한 순서로 뽑았습니다.\n")
    return answer


def get_guess():
    print("숫자 3개를 하나씩 차례대로 입력하세요.")
    guess = []

    # 코드 작성

    return guess


def get_score(guess, solution):
    strike_count = 0
    ball_count = 0

    # 코드 작성

    return strike_count, ball_count

def main():
    tries = 0
    answer = generate_answer()

    while 1:
        guess = get_guess()
        strike, ball = get_score(guess, answer)
        print("{}S {}B ".format(strike, ball))

        if strike == 3:
            tries += 1
            break
        else:
            tries += 1

    print("축하합니다. {}번 만에 숫자 3개의 값과 위치를 모두 맞추셨습니다.".format(tries))

if __name__ == "__main__":
    main()

```
