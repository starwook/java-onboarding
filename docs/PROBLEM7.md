## 🚀 기능 요구 사항

레벨 2의 팀 프로젝트 미션으로 SNS(Social Networking Service)를 만들고자 하는 팀이 있다. 팀에 속한 크루 중 평소 알고리즘에 관심이 많은 미스터코는 친구 추천 알고리즘을 구현하고자 아래와 같은 규칙을 세웠다.

- 사용자와 함께 아는 친구의 수 = 10점 
- 사용자의 타임 라인에 방문한 횟수 = 1점

사용자 아이디 user와 친구 관계 정보 friends, 사용자 타임 라인 방문 기록 visitors가 매개변수로 주어질 때, 미스터코의 친구 추천 규칙에 따라 점수가 가장 높은 순으로 정렬하여 최대 5명을 return 하도록 solution 메서드를 완성하라. 이때 추천 점수가 0점인 경우 추천하지 않으며, 추천 점수가 같은 경우는 이름순으로 정렬한다.

### 제한사항

- user는 길이가 1 이상 30 이하인 문자열이다.
- friends는 길이가 1 이상 10,000 이하인 리스트/배열이다.
- friends의 각 원소는 길이가 2인 리스트/배열로 [아이디 A, 아이디 B] 순으로 들어있다.
  - A와 B는 친구라는 의미이다.
  - 아이디는 길이가 1 이상 30 이하인 문자열이다.
- visitors는 길이가 0 이상 10,000 이하인 리스트/배열이다.
- 사용자 아이디는 알파벳 소문자로만 이루어져 있다.
- 동일한 친구 관계가 중복해서 주어지지 않는다.
- 추천할 친구가 없는 경우는 주어지지 않는다.

### 실행 결과 예시

| user | friends | visitors | result |
| --- | --- | --- | --- |
| "mrko" | [ ["donut", "andole"], ["donut", "jun"], ["donut", "mrko"], ["shakevan", "andole"], ["shakevan", "jun"], ["shakevan", "mrko"] ] | ["bedi", "bedi", "donut", "bedi", "shakevan"] | ["andole", "jun", "bedi"] |

## 🚀 기능 목록
1. 유저의 친구목록을 리스트로 만들어주는 메소드
2. 제공되는 친구 리스트를 탐색해, 두 문자열중 유저의 친구가 하나 포함되어있으면 다른 문자열을 친구 추천 점수 Map에 넣어주거나,10점을 더해주는 메소드(여기서 다른 문자열은 유저일땐 스킵)
3. 제공되는 방문자 리스트를 탐색해, 친구추천점수Map에 넣어주거나,1점 올리는 메소드
4. 정렬을 하기 위해 리스트로 친구추천점수Map을 친구추천점수List로 바꿔주는 메소드
5. 친구추천 점수List를 버블솔트를 사용해 1순위는 점수 내림차,2순위는 알파벳 오름차순으로 정렬해주는 메소드
6. 정렬된 친구추천점수리스트에서 이름만을 정답리스트에 차례대로 넣어주는 메소드