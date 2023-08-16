# SimpleChat
#### ⚪ About Project
* ##### 웹소켓을 사용한 실시간 채팅 구현
* ##### NestJS, 웹소켓 게이트웨이를 통해 서버와 클라이언트간 양방향 통신 지원
* * *
#### ⚪ Usage
https://www.youtube.com/watch?v=1UvK-YwjQaA
  <img src="https://user-images.githubusercontent.com/79093184/260901610-e7dab1f5-c9ab-4a7d-be95-96130f604c49.png" align="center">

* * *
#### ⚪ Built With
<img alt="Html" src ="https://img.shields.io/badge/HTML5-E34F26.svg?&style=for-the-badge&logo=HTML5&logoColor=white"/> <img alt="Html" src ="https://img.shields.io/badge/NestJS-E0234E.svg?&style=for-the-badge&logo=NestJS&logoColor=white"/> <img alt="Html" src ="https://img.shields.io/badge/TypeScript-3178C6.svg?&style=for-the-badge&logo=TypeScript&logoColor=white"/>

* * *
#### ⚪ Getting Strated
* ##### Prerequisites: npm, node, MongoDB Connection URL
* ##### Installation & Execution
```bash
git clone https://github.com/MpqM/WebApp_Board.git
# Change the MONGO_CONNECTION_STRING value in the configs/mongodb-connection.jsfile with yours
npm install
npm start
```
* * *
#### ⚪ Description
* ##### express-handlebars: 자바스크립트 view 템플릿을 이용해 헬퍼 함수를 작성하고 이용
* ##### Post
   * ##### 게시글 작성시 비밀번호 해쉬 처리후 DB저장
   * ##### 게시글 상세보기를 통해 게시물 정보(댓글, 작성자, 작성일자 등)확인
   * ##### 게시글 수정, 삭제시 check-pasword API 을 통해 비인가적인 삭제 호출 막음
* ##### Comment
   * ##### DB의 Post에 배열 형식으로 Post DB에 존재 
   * ##### 댓글 작성시 비밀번호 해쉬 처리후 Post DB destruct 후 저장
   * ##### 댓글 삭제시 2중 쿼리사용 API를 통해 비밀번호 인증후 삭제
* ##### List
    * ##### 리스트에서 게시글 검색 및 페이지 네이션 api
    * ##### 페이지네이션구현 -> utils/paginator.js 참조
* ##### RESTAPI
    * ##### Post: 게시글 생성, 삭제, 수정, 상세보기 기능
    * ##### Comment: 댓글 삭제, 생성 기능
    * ##### List: 홈페이지 요청처리 게시글 목록, 조회, 페이지네이션 기능
    * ##### 자세한 내용은 app.js 주석 참조
* * *
#### ⚪ Roadmap & Realization & Study
* ##### Node.js 백엔드 개발자 되기 chapter7의 프로젝트를 보고 따라함
* ##### 자바스크립트 템플릿 엔진인 express-handlebars에 대해 실습
* ##### 실습 프로젝트 내용에는 비밀번호 인증이지만 DB에 그대로 평문이 저장됨
* ##### 이에 bcrypt 패키지를 통해 암호화 기능을 적용해 DB에 저장되는 비밀번호에 해쉬적용
* ##### 비밀번호 인증시 해쉬 비교 수행후 인증 확인/거부
* ##### 디렉토리 재구조화 MVC 패턴
* ##### MongoDB 정규식 표현이 미숙해 댓글(post.comments)에 접근하는데 비동기호출을 2번사용함
* * *
#### ⚪ Writer
* ##### <span>okqkrwhdtjd@gmail.com
* <a href = "https://github.com/MpqM"><img alt="GitHub" src ="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/></a> <a href = "https://MpqM.tistory.com/"> <img alt="Tistory" src ="https://img.shields.io/badge/Tistory-white.svg?&style=for-the-badge"/></a>
* * *
#### ⚪ Contributing
* ##### Fork the Project https://github.com/MpqM/WebApp_Board
* ##### Create your Feature Branch (git checkout -b feature/AmazingFeature)
* ##### Commit your Changes (git commit -m 'Add some AmazingFeature')
* ##### Push to the Branch (git push origin feature/AmazingFeature)
* ##### Open a Pull Request
* * *
#### ⚪ Acknowledgments & License & reference
* ##### https://github.com/wapj/jsbackend/tree/main/chapter7
* ##### 박승규,『Node.js 백엔드 개발자 되기』, GOLDENRABBIT, p234~293
* * * *
