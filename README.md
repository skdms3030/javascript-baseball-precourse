<p align="middle" >
  <img width="200px;" src="https://github.com/woowacourse/javascript-baseball-precourse/blob/main/images/baseball_icon.png?raw=true"/>
</p>
<h1 align="middle">숫자 야구 게임</h1>

##기능 목록

1. 정답 생성
- 1~9 사이의 임의의 정수 3개
- 중복되지 않음
- MissionUtils 라이브러리의 Random.pickNumberInRange 사용

2. 사용자의 입력값받기
- 중복된 값 입력 -> 에러메세지 alert
- 숫자가 아닌 값 입력 -> 에러메세지 alert
- 1~9가 아닌 값 입력 -> 에러메세지 alert

3. 볼, 스트라이크 갯수 세기
- 입력값 한글자씩 검사
	  정답에 포함된 숫자이지만 위치가 다를 경우 -> 볼갯수++
	  정답과 같은 위치에 있는 같은 숫자일 경우 -> 스트라이크갯수++

4. 결과텍스트 판단
결과텍스트는
- 스트라이크 갯수가 3인 경우 -> 정답
- 볼 갯수가 0이고 스트라이크 갯수가 0이 아닌 경우 -> ${스트라이크갯수}스트라이크
- 볼 갯수가 0이 아니고 스트라이크 갯수가 0일 경우 -> ${볼갯수}볼
- 볼 갯수가 0이 아니고 스트라이크 갯수가 0이 아닐 경우 -> ${볼갯수}볼 ${스트라이크갯수}스트라이크
- 볼 갯수가 0이고 스트라이크 갯수가 0일 경우 -> 낫싱

5. 결과텍스트 출력
5-1. 정답이 아닐 경우
- 결과 텍스트를 결과창에 출력

5-2. 정답일 경우
- '정답입니다'와 재시작버튼를 결과창에 출력
- 재시작 버튼 클릭시
	  입력창과 결과창 비우기
	  새로운 정답 생성