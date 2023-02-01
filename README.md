# ToyProject-YouTube-Clone

### 개발 기간
- 23년 1월 16일 ~ 23년 1월 20일

<br />

### 데모 사이트
- [YouTube Clone](https://toy-youtube-clone-t3.netlify.app)

<br />

## 팀원 소개 및 역할 분담
|**[노준영](https://github.com/ghgt1)**|**[박정민](https://github.com/plou102)**|**[조민정](https://github.com/quokka-eating-carrots)**|
|:---:|:---:|:---:|
|<img src='https://avatars.githubusercontent.com/u/35508595?v=4' width='150'>|<img src='https://avatars.githubusercontent.com/u/107393773?v=4' width='150'>|<img src='https://avatars.githubusercontent.com/u/113992260?v=4' width='150'>|
|재생 페이지 <br /> 헤더|메인 페이지 <br />검색 페이지|재생 페이지 <br /> 사이드 바|

<br />

## 기술 스택

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white)
![CSS Modules](https://img.shields.io/badge/CSS_Modules-000000?style=for-the-badge&logo=css-modules&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)

## 주요 구현 사항

##### 제가 100% 구현한 내용들로만 작성하였습니다.

- Youtube API를 활용하여 원본 유튜브의 기능들을 그대로 구현하고자 노력하였습니다.
- Header를 반응형으로 구현하였습니다

- 원본 Header입니다

<p align="center">

![image](https://user-images.githubusercontent.com/35508595/215948118-269b99a8-4f81-478d-b674-0d7105a7bb0f.png)
</p>

- 모바일 태블릿 환경에서의 Header입니다 

<p align="center">

![image](https://user-images.githubusercontent.com/35508595/215951494-4e287e76-d6d8-4743-9462-fc8c401a64bd.png)
</p>

- 검색버튼을 클릭할시, 다음과 같이 변하게 됩니다.

<p align="center">

![image](https://user-images.githubusercontent.com/35508595/215948251-8399a853-00bc-4a98-b1b0-b7b9cd3725ea.png)
</p>

- React Responsive라이브러리를 활용하여 Media query 브레이크포인트 설정을 동적으로 JS에서 할수있었습니다. 따라서 state의 변화를 감지하여 그에 맞게 렌더링하였습니다.

- 재생페이지 진입시 좌측 Nav바가 자동으로 들어가게 구성하였습니다. 이때, 전역 상태관리 라이브러리를 따로 활용하지 않아서 Props drilling이 필요했는데 Outlet으로 구성되어있는 요소에게 Props를 넘기는 방법에 대해 고민해보았고 `useOutletContext` 라는 기능을 활용하여 Outlet요소에도 props값을 넘길수있었습니다.

- 재생페이지 우측의 관련동영상과 하단의 댓글기능을 구현하였습니다. Youtube API의 요청횟수가 많이 부족하여, 무한스크롤이나 추가적으로 불러오는 기능은 넣지않고, 각각 10개, 20개씩만 불러오게 구현해놓았습니다.

- 반응형으로 구성하여 태블릿 모바일 환경에서는 관련동영상의 위치를 아래로 조정해주었습니다. 이때는 CSS의 media query를 사용하였습니다.



