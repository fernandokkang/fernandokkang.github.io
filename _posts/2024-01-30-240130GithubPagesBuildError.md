---
layout: single
title: "Github Pages Build Error - Liquid Exception: Liquid syntax error"
categories: Solution
tag: [Github Pages]
toc: true
---

### 에러 내용
```
  Liquid Exception: Liquid syntax error (line 10): Variable '{ {1, 2, 3}' was not properly terminated with regexp: /\}\}/ in /github/workspace/_posts/2024-01-30-240130DailyQuiz.md
```

### 에러 원인
 10번째 행에 배열 선언 부분을 정규 표현식으로 인식하여 오류가 발생하였음.
 
### 해결 방법
 배열 선언 앞 뒤로 공백을 넣어준다
 ```
    int[][] a = { {1, 2, 3}, {4, 5, 6} };
 ```