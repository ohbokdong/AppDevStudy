# 프로젝트 진행상황 공유 0830 (ch.choi)

## 프로젝트 진척상황
_____

* 클라이언트 -> 서버 전송 단방향 통신 더미 완료 (n:1)


## 기존 이슈 해결
_____

* ~~SOCKET을 이용한 프로그래밍 진행 시 링커 에러 발생~~
  * lib 참조가 안되서 에러 발생, ws2_32.lib 참조하여 에러 해결


## 이슈 
_____

* 지정된 수의 클라이언트가 접속을 하길 기다려야 함 (Accept는 블로킹 함수)
  * 예 : 2명이 접속 해야 서버 실행 가능
* 서버에 연결된 클라이언트 순서에 따라 결과가 출력이 됨 (클라2 입력, 클라1 입력: 서버 출력순서 클라 1, 클라2 출력 ,  클라2 입력 : 서버 출력 x)
  * 반복문을 통해 순차적으로 Recv를 받다 보니 우선 순위가 생김
  * 클라이언트 순서 상관 없이 서버에서 데이터 받을 수 있도록 수정 필요


## 다음주 목표(TO DO)
_____

* 논블로킹 방식 도입 여러 클라이언트 접속 가능 하도록 변경
* 클라이언트 데이터 전달 받을 수 있도록 구현
* 콘솔 더미 제작




[블로킹 함수 설명](https://homoefficio.github.io/2017/02/19/Blocking-NonBlocking-Synchronous-Asynchronous/)

