## RESTful API using MongoDB & Mongoose & Express
VELOPERT 블로그에 작성한 강좌에 사용된 프로젝트 입니다.  
MongoDB, Mongoose 와 Express 를 사용하여 간단한 RESTful API 를 구현합니다.  
 
 
 
 해야 할 일
 ### 1. 프로젝트 생성 및 패키지 설치
 1-1) 프로젝트 생성
 npm init 을 통해 package.json 생성하기 설정 값은 default 값으로 하면 됨
 $ npm init
 
 1-2) 패키지 설치
 이번 프로젝트에서 사용할 패키지
    1. express : 웹프레임워크
    2. body-parser : 데이터 처리 미들웨어
    3. mongoose : MongoDB 연동 라이브러리
 $ npm install --save express mongoose body-parser
 
 명령어 입력 시 자동으로 패키지 설치하고, package.json 파일에 패키지 리스트를 추가한다.
 
 ### 실행 법
 1-1) 서버와 DB 연동하기
  1. mongod --dbpath 파일 경로
  2. mongo
  3. node 서버 실행 파일 확장자까지 입력
  
 local host adress 설정한대로
 POST | http://localhost:8080/api/books/
 GET  | http://localhost:8080/api/books/

... (API 목록 참고)
 
 
 ## login directory
 개발 환경 동일
 id, password 입력 시 
 입력사항 출력 시키는 html 가시화
 password type 'text' 가 아닌 password 사용시 쿠기 저장 됨
 
 

### API 목록
| ROUTE                     | METHOD | DESCRIPTION               |
|---------------------------|--------|---------------------------|
| /api/books                | GET    | 모든 book 데이터 조회     |
| /api/books/:book_id       | GET    | _id 값으로 데이터 조회    |
| /api/books/author/:author | GET    | author 값으로 데이터 조회 |
| /api/books                | POST   | book 데이터 생성          |
| /api/books/:book_id       | PUT    | book 데이터 수정          |
| /api/books/:book_id       | DELETE | book 데이터 제거          |

링크: https://velopert.com/594
