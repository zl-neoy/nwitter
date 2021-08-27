- 실전형 리액트 Hooks 10개 듣기
## 0. INTRODUCTION
### 0.3 When To Use Firebase
- 굉장히 빠르게 무언가를 할 수 있음
- 진입이 쉬움
- 실제 프로젝트에는 불가
- 이걸 쓰면 거의 구글로부터 빌려서 쓰는 거
- 걍 시작할 때 사용, 그냥 테스트
- 빠르게 무언가를 하랴고 할 때 그냥 규모있게만 
- 비즈니스 용도로는 파베 사용 안 할 거임. 걍 구상할 때만 

### 0.4 Pricing in Firebase
- 파베 무료 아님
- 무거운 거 비용 지불 해야함
---
## 1 SETUP
### 1.0 React + Firebase Setup
- ```npx create-react-app nwitter```
- ```npm install --save firebase```
- 프로젝트를 만들었는데 기본적으로 Firebase Web의 형태, application도 만듦
- Firebase 설치, 파일을 하나 만들어서 firebase의 initialization까지도 진행

### 1.1 Securing the Keys
- .env 파일 생성 : 모든 key와 URL을 코드에 적어놓는 거 대신에 .env 파일을 생성함. 환경 변수가 담겨져 있음
- react.js applicaton을 사용한 경우 (create-react-app을 사용한 경우) -> REACT_APP으로 시작해야하고 그 뒤로 이름을 붙여줘야 함.
```REACT_APP_SOMETHING``` : REACT_APP으로 시작하는 환경변수를 찾도록 자동으로 설정이 되어 있음.
- 왜 .env 파일을 따로 만드냐? gitignore에 쓸 수 있음. .env파일은 git으로부터 무시됨 (git의 버전 관리 대상에 포함되지 않음) 
- 하지만 완전히 보안할 수 있는 것은 아님. 내가 react application을 실행하면  결국에는 이 값들이 들어가게 됨. 그렇지 않으면 firebase에 접근하지 못함
걍 github에만 못 올라가도록.
- .env파일은 프로젝트의 최상위에 있어야함.  

### 1.2 Router Setup (구조 잡기)
- route를 사용하기 위해서 ```npm i react-router-dom``` 으로 설치
- HashRouter가 뭘까..?
- 렌더시칼 routes는 인증여부에 따라 달라질 ㄹ예정
- useState는 기본적으로 False여야 함.
- 자동으로 import되기를 원한다면 const Auth = () => {} 처럼 사용
- fragment : 많은 요소를 render하고 싶을 때 사용(부모 요소가 없을 때) <>  </>
---
## 2. AUTHENTICATION
### 2.0 Using the Firebase Auth
### 2.1 Login Form part One
### 2.2 Recap
### 2.3 Creating Account
### 2.4 Log In
### 2.5 Social Login
### 2.6 Log Out

## 3. NWEETING
### 3.0 Form and Database Setup
### 3.1 Nweeting!
### 3.2 Getting the Nweets
### 3.3 Realtime Nweets
### 3.4 Delete and Update part One
### 3.5 Delete and Update part Two
### 3.6 Recap
---
## 4. FILE UPLOAD
### 4.0 Preview Images part One
### 4.1 Preview Images part Two
### 4.2 Uploading
### 4.3 File URL and Nweet
### 4.4 Deleting Files
---
## 5. EDIT PROFILE
### 5.0 Get My Own Nweets
### 5.1 Update Profile
### 5.2 Update Profile Bugfix
---
## 6. FINISHING UP
### 6.0 Cleaning JS
### 6.1 Styles
### 6.2 Deploying
### 6.3 Security on Firebase
### 6.4 API key Security
### 6.5 Conclusions

|강의| 날짜 | 들었냐 |   
|-|-|:-:|
|챕터 0|8.26|O| 
|챕터 1, 2, 3|8.27| O / /|
|챕터 4, 5, 6|8.28| / / |
