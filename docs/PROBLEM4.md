## 🚀 기능 요구 사항

어느 연못에 엄마 말씀을 좀처럼 듣지 않는 청개구리가 살고 있었다. 청개구리는 엄마가 하는 말은 무엇이든 반대로 말하였다.

엄마 말씀 word가 매개변수로 주어질 때, 아래 청개구리 사전을 참고해 반대로 변환하여 return 하도록 solution 메서드를 완성하라.

| A | B | C | D | E | F | G | H | I | J | K | L | M | N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Z | Y | X | W | V | U | T | S | R | Q | P | O | N | M | L | K | J | I | H | G | F | E | D | C | B | A |

### 제한사항

- word는 길이가 1 이상 1,000 이하인 문자열이다.
- 알파벳 외의 문자는 변환하지 않는다.
- 알파벳 대문자는 알파벳 대문자로, 알파벳 소문자는 알파벳 소문자로 변환한다.

### 실행 결과 예시

| word | result |
| --- | --- |
| "I love you" | "R olev blf" |



## 🚀 기능 목록
1. 주어진 문자열의 문자를 하나하나 2번 메소드의 인수로 넣어줘 최종 String을 받는 메소드
2. 주어진 문자가 알파벳인지 아닌지 3번 메소드로 확인하여 아니라면 그대로 돌려주고 아니라면 4번 메소드의 반환값을 돌려주는 메소드
3. 알파벳인지 아닌지 확인하는 메소드
4. 아스키코드 따라서 소문자,대문자를 구분하여 5번메소드에 155또는 219를 넣어주는 메소드(대문자일땐 65+90 =155 ,소문자일땐 97+ 122= 219를 넣어줌)
5. 주어진 숫자에서 주어진 문자를 뺴서 반환하는 함수(아스키코드 기준으로 대칭임으로, 빼서 알파벳 변환하는 식)
