# boiler-plate-ko
노드 리액트 기초 강의 boiler-plate

https://www.youtube.com/playlist?list=PL9a7QRYt5fqkZC9jc7jntD1WuAogjo_9T


## 8 Nodemon
npm install nodemon --save-dev

## 9 비밀 정보 보호
X

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

## 15 React
What is React JS?
1. Library
2. Components, reusable이 뛰어남
3. Virtual DOM

Babel : 최신 JS문법을 구형 브라우저에서 돌 수 있게 변환 시켜줌.
Webpack : Javascript Application의 Static Module Bundler

## 16 Create-React-App
npx create-react-app .

## 17 npm & npx
npm : Node.js의 의존성과 패키지 관리를 위한 패키지 매니저

npx : Node 패키지를 실행시키는 하나의 도구, 실행 할 때마다 최신 버전의 모듈을 불러와서, 설치 하고 다시 그 모듈을 삭제하는 방식

## 18 구조 설명
X

## 19 CRA to Our BoilerPlate
#### src폴더 구조 - BoilerPlate 특성화된 구조
* _actions : Redux를 위한 폴더
* _reducer : Redux를 위한 폴더
* components/views : Page들을 넣는다.
* components/views/Sections : 해당 Page에 관련된 css, component 등을 넣는다.
* App.js : Routing 관련 일을 처리한다.
* Config.js : 환경 변수 등을 정하는 곳
* hoc : Higher Order Component
* utils : 여러 군데에서 쓰일 수 있는 것들을 넣는다.

#### 확장프로그램
* ES7 React/Redux/GraphQL/React-Native snippets : rfce, rcc 등

## 20 React Router Dom
https://reactrouter.com/web/guides/quick-start

페이지 이동을 할 때 React Router Dom이라는 것을 사용한다.

## 21 데이터 Flow & Axios

npm install axios --save

## 22 CORS 이슈, Proxy 설정
#### Cross-Origin Resource Sharing
CORS정책 때문에
두 개의 다른 포트를 가지고 있는 서버는 아무 설정없이 Request를 보낼 수 없다.

#### Proxy 설정
https://create-react-app.dev/docs/proxying-api-requests-in-development

npm install http-proxy-middleware --save

## 23 Proxy Server ?
#### Proxy Server란
[User] ⇔ [Proxy Server] ⇔ [Internet]
1. IP를 Proxy Server에서 임의로 바꿀 수 있다.
2. 보내는 데이터도 임의로 바꿀 수 있다.
3. 방화벽 기능
4. 웹 필터 기능
5. 캐시 데이터, 공유 데이터 제공 기능

#### Proxy Server 사용 이유!
1. 회사에서 직원들이나 집안에서 아이들 인터넷 사용 제어
2. 캐시를 이용해 더 빠른 인터넷 이용 제공
3. 더 나은 보안 제공
4. 이용 제한된 사이트 접근 가능

## 24 Concurrently
여러 개의 commands를 동시에 작동시킬 수 있게 해주는 Tool
ex) 프론트, 백 서버를 동시에 켜기

npm install concurrently --save
```js
"start": "concurrently \"command1" \"command2\""
```

## 25 Antd CSS Framwork
#### CSS Framwork를 사용하는 이유
기능을 만드는 데 더욱 집중하기 위해서

#### CSS Framwork 종류 For ReactJS
1. Material UI
2. React Bootstrap
3. Semantic UI
4. Ant Design
5. Materialize

#### Antd Design
http://ant.design/

npm install antd --save
