# boiler-plate-ko
노드 리액트 기초 강의 boiler-plate
https://www.youtube.com/playlist?list=PL9a7QRYt5fqkZC9jc7jntD1WuAogjo_9T


## 8 Nodemon
npm install nodemon --save-dev

## 9 비밀 정보 보호

## 10 Bcrypt로 비밀번호 암호화 하기
Bcrypt를 이용하여 비밀번호를 암호화 후 DB에 저장

https://www.npmjs.com/package/bcrypt

npm install bcrypt --save

## 11 로그인 기능 with Bcrypt
로그인 기능 구현
1. 요청된 Email을 DB에서 찾기
2. 요청된 Email이 DB에 있다면 PW확인
3. PW가 맞다면 토큰 생성

## 12 토큰 생성 with jsonwebtoken
https://www.npmjs.com/package/jsonwebtoken

npm install jsonwebtoken --save

npm install cookie-parser --save

## 13 Auth 기능 구현
auth route 구현
1. 페이지 이동 때마다 로그인되어 있는지, 관리자 유저인지 등을 체크
2. 글을 쓸 때나 지울 때 등에 권한이 있는지 체크

## 14 로그아웃 기능
로그아웃 route 구현
1. 로그아웃하려는 유저를 DB에서 찾는다.
2. 해당 유저의 토큰을 삭제한다.
