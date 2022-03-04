# Backjoon for JS

자바스크립트로 백준 온라인 저지 문제를 풀도록 돕는 레포지토리입니다.

코드 템플릿 및 추천 문제를 제공합니다.

### Template

- JS는 브라우저 환경에서 작동하므로 백준 사이트의 문제를 풀기 위해서는 Node JS 를 사용해야 합니다.
- Node JS로 코드를 작성하기 위해 다음의 두 가지 템플릿을 권장드립니다.

**basic**

```js
const fs = require('fs');
// TODO: 제출 시 경로 변환 필수 ("/dev/stdin")
const input = fs.readFileSync('test.txt').toString().trim().split('\n');

// 풀이
function solution(arr) {
  const [a, b] = arr[0].split(' ');
  return Number(a) + Number(b);
}

console.log(solution(input));
```

**extended**

```js
const fs = require('fs');
// TODO: 제출 시 경로 변환 필수 ("/dev/stdin")
const input = fs.readFileSync('test.txt').toString().trim().split('\n');
// 정리
/* ex.
const x = Number(input[0]);
const [y, z] = input[1].split(' ').map(v => Number(v));
const arr = input[2].split(' '); 
*/
// 풀이
function solution(x, y, z, arr) {
  const answer = [];
  return answer.join('\n');
}

console.log(solution(x, y, z, arr));
```

- 테스트 케이스는 `test.txt`에 작성하여 노드 환경에서 동작시킬 수 있습니다. (ex. `node my-solution.js`)
- 제출 시 경로는 `test.txt`에서 `/dev/stdin`으로 변경해야 정상적으로 채점이 이루어집니다.
- input변수에 각 라인을 나누어 배열로 저장합니다.
- extended 템플릿의 경우 solution 함수에 넣기 전 미리 정리하는 방식입니다. 이를 통해 다른 PS 플랫폼과 유사하게 문제를 풀 수 있습니다.
- 답이 한 줄일 경우 basic의 return처럼 작성합니다.
- 여러 줄일 경우 반드시 extended의 return과 같이 배열내에 답을 넣어 `join('\n')`으로 하나의 string으로 만들어야 합니다.

### Suggest

- 코딩 테스트에 주로 나오는 유형을 정리하였습니다.
- JS를 완전히 지원하지 않는 백준 플랫폼 특성상 다음의 기준에 적합한 문제들을 선별하였습니다.
  - 맞힌 사람 3,000명 이상
  - JS로 푼 사람 10명 이상
- 각 링크를 클릭하여 해당 문서로 이동할 수 있습니다.

| Title                 | Name                 | Count | Link |
| --------------------- | -------------------- | ----- | ---- |
| Implementation        | 구현                 | 0     |      |
| Dynamic Programming   | 동적계획법           | 0     |      |
| Bruteforce            | 브루트포스           | 0     |      |
| Sorting               | 정렬                 | 0     |      |
| Binary Search         | 이분 탐색            | 0     |      |
| BFS & DFS             | 너비 & 깊이 우선탐색 | 0     |      |
| Prefix Sum            | 누적합               | 0     |      |
| Dijkstra              | 다익스트라           | 0     |      |
| Disjoint Set          | 분리 집합            | 0     |      |
| Backtracking          | 백 트래킹            | 0     |      |
| Stack & Queue         | 스택 & 큐            | 0     |      |
| Two Pointer           | 투 포인터            | 0     |      |
| Minimum Spanning Tree | 최소 스패닝 트리     | 0     |      |
| Topological Sorting   | 위상 정렬            | 0     |      |
| Floyd-warshall        | 플로이드 와샬        | 0     |      |
| Sliding Window        | 슬라이딩 윈도우      | 0     |      |

### Contributor

|           [harry](https://github.com/haesoo9410)           |
| :--------------------------------------------------------: |
| <img src="https://github.com/haesoo9410.png" height="100"> |

- 기준에 적합한 문제는 언제든 PR을 남겨주세요.
- 커밋 컨벤션은 [깃모지](https://haesoo9410.tistory.com/301)를 따르고 있으며 지키지 않아도 좋습니다.
- 그 외 제안할 내용이 있다면 ISSUE를 작성해주세요.
