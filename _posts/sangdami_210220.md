---
title: 상다미-210220
date: 2021-02-20
tags:
  - sangdami
  - logout
  - profile
---

### to-do

- [x] profile 클릭시, profile 페이지(유저 정보 표시)
- [x] logout 하면 유저 정보를 모두 삭제(cookie, session)

### profile

- `req.user` 통해서, user name, email 정보를 받기
- controller에서 위 정보를 pug로 넘겨서, 해당 유저 정보 표기

### logout

- `req.logout()`이라는 매우 좋은 passport function 쓰면 됨
- 자동으로 유저 정보 삭제! 굳
