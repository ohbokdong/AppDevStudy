## 프로젝트 진척상황 공유5 (minj0i) - 2020-10-25
- 자격증 및 기타 시험 등으로 너무 바빴다.
- 준비가 안된 상태에서 뭔가 해보려고 하니 더 힘들었다. (마치 갯벌에서 허우적 거릴수록 더 깊이 빠지는 것 같은 느낌..-> 알려주고 싶었음ㅜㅜ)
- uuid 관련해서 getDeviceInfo를 사용하려고 했었는데, 좀 더 검색해보니 좀 간단한게 있었음
- 코드를 어디에 넣느냐에 따라서 값이 뭔가 계속 변경되면서 찍히고 있는데 확인 필요
```
npm install react-native-uuid
```

```
import uuid from 'uuid/v1';   //v4 를 사용하고 싶으면 uuid/v4 해주면 됩니다
console.log(uuid(););    // 시간기반으로 생성된 32자리의 16진수가 console창에 출력됩니다.
```

## 다음 주 일정
- 분기처리
    - 처음 시작 시 : 시작 버튼 누르면 uuid 이름으로 collection 추가
    - 이후: uuid 불러와서 data 추가/삭제
- 디자인 예쁘게