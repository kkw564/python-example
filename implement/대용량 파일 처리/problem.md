### 문제

당신은 오랜 시간 동안 매일의 생각과 일어난 일을 기록해 온 대용량의 일기장 파일(`diary.txt`)을 가지고 있습니다.
일기장의 각 줄은 날짜와 그 날의 일기 내용으로 구성되어 있으며, 다음과 같은 형식을 가집니다: `YYYY-MM-DD 일기 내용`.
오늘은 일기장을 정리하는 날인데 일기장에서 특정 키워드별 단어가 몇번 나왔는지 정리해보고싶습니다.
즉, 일기 내용 중에서 `"행복", "기쁨", "슬픔", "분노"`가 일기에서 각각 몇번 포함된지 찾아보는 프로그램을 만들어보세요.

### 구현 팁

"행복"이 1번
"기쁨"이 10번
"슬픔"이 3번
"분노"가 40번
인 경우 아래와 같이 형성하여 ans == diary_ans를 비교하면 됩니다.

```python
ans = {
  "행복": 1,
  "기쁨": 10,
  "슬픔": 3,
  "분노": 40
}
```
