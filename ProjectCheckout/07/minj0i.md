# 프로젝트 진척상황 공유7 2020-11-31

- 지수언니가 보내준 운동어플에서 힌트를 얻어 깃 오픈소스를 검색하니
  - git heatCalendar라는 이름들로 여러 오픈소스들이 나왔다
  - https://cal-heatmap.com/
  - https://github.com/Bloggify/github-calendar
- 기왕 시작한거 그냥 혼자 다 해보는거로 결정

- 초기화면 만듬
- styled component를 쓰니깐 변경도 잘 안되고 별로인 것 같다(장점을 아직 못찾음)
- 갤럭시S20+랑 갤럭시S9으로 테스트했다
  - scroll 때문에 고정 height이 필요한데 어떻게 할지 고민
  - px에서 %로 변경하고, 일단 전체 View에 height:100%를 주니 넘치진 않는다