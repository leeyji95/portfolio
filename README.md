## 이예지 포트폴리오
<br>

* * *
# SPRING 팀프로젝트 2

#### 소스코드 및 시연영상
* 서점관리시스템ERP Yes25_ver2 (소스코드)   
[.java] (https://github.com/leeyji95/Yes25_ver2/tree/master/src/main/java/com/lec/yes25/personnel)   
[Mybatis mapper] (https://github.com/leeyji95/Yes25_ver2/blob/master/src/main/java/com/lec/yes25/mapper/PersonnelDAO.xml)   
[ERD 테이블 및 sql 쿼리] (https://github.com/leeyji95/Yes25_ver2/blob/master/src/main/webapp/ERD/personnel/final.sql)   
[JS 코드] (https://github.com/leeyji95/Yes25_ver2/tree/master/src/main/webapp/JS/personnel)   
[Spring Security 관련 컨텍스트] (https://github.com/leeyji95/Yes25_ver2/blob/master/src/main/webapp/WEB-INF/spring/appServlet/security-context.xml)   

* 서점관리시스템ERP Yes25_ver2 (발표시연 영상)   
[파트 시작: 4분01초 ~ 끝: 9분27초] (https://youtu.be/DlhkyodF7ig?t=241)   

#### 발표 일자 
* 2020/08/05 발표

#### 개요
* 서점 직원 인사관리를 비롯한, 제품, 물류, 구매, 재무관리를 한눈에 보기 쉽고 빠른 접근성을 위한 서점관리 시스템 ERP이며,   
  비동기식 SPA 로 구현한 애플리케이션입니다.


#### 공헌한 내용
* 참여도: **40%**
* 팀장역할   
  DB ERD 테이블 설계 및 취합, DDL, DML 작성,   
  스토리보드 작성 흐름도 및 구성도 작성 및 취합,   
  이클립스 셋팅, Git 셋팅 및 공유 / 깃 에러처리,   
  전제적인 html, css 이용한 디자인템플릿 배포, 프로젝트 관리   
* 맡은 파트 :  로그인/로그아웃 처리 구현, 신규사원등록, 출퇴근등록 구현, 근태현황조회 페이지 구현   
  1) 로그인/로그아웃 : Spring Security 사용   
  intercept-url pattern 사용하여 특정 url 접근권한 제한   
  JSTL c 태그의 namespace sec 사용하여 권한에 따른 보기 설정   
  로그인 성공 핸들러, 로그아웃 처리시 세션 삭제 처리   
  PasswordEncoder 사용하여 비밀번호 암호화 처리   
  jdbc 연동 하여 시큐리티 사용 jdbc-user-service 사용   
  2) 사원 출퇴근 등록 Ajax 처리 구현   
  출근 등록 클릭 시 => DB 에 출근시각 , 근무상태 INSERT   
  오전 9시 기준 이전 		        : 정상출근   
	오전 9시 이후 ~ 오후 12시 이전  : 지각처리   
	오후 12시 이후 ~ 		          : 결근처리   
  퇴근 등록 클릭 시 => DB 에 퇴근시각 , 근무상태, 총 근무시간 UPDATE   
  결근인 경우        : 결근처리   
  오후 6시 기준 이전 : 조퇴처리   
	오후 6시 이후      : 정상퇴근   
  3) 신규사원등록 : Ajax 처리 구현      
  Js jQuery 라이브러리 이용, form 태그 Serialize 하여 Ajax로 요청처리   
  Ajax로 request 요청 시 header 에 Security 사이트 위조 방지를 위한 csrf-token 처리   
  4) 근태현황조회 페이지 구현   
  출퇴근 등록 시 insert 및 update 된 테이블의 모든 컬럼 값들을 SELECT 하도록 Ajax 처리   
  <br>
* 웹 화면 구성 : HTML5, CSS3, BootStrap, JavaScript, jQuery, DatePicker   
* 결과를 얻어오기 위한 서버 액션 : JAVA, Spring MVC2, Restful API, JSTL, EL   
* DB액션 처리 : JDBC, mybatis   
* 사용기술: HTML5, CSS3, JavaScript, jQuery, JSON, Ajax, BootStrap4.0, Java,   
           Spring4, Spring Tool Suite(STS4), Spring Security, Maven, JSTL, EL,   
           JDBC, Oracle 11g, Apache Tomcat9.0, DatePicker   <br>

#### 사용 Tool
* ERD 설계와 DDL 작성: AQueryTool, DBeaver   
* Flow Chart 작성: Draw.io   
* 개발환경: Eclips, Apache Tomcat v9.0, Visual Studio Code, Oracle 11g   
* 협업툴: GitHub

<br>
<br>
<br>

* * *
* * *

# JSP 팀프로젝트 1

[개발자 커뮤니티 Sysout (소스코드)] (https://github.com/writerkang/Maxim_Project)   
[개발자 커뮤니티 Sysout (발표시연 영상)] (https://youtu.be/c5x5BAcvOAE?t=438)   
(파트 시작: 7분17초 ~ 끝: 13분) 

#### 발표 일자 
* 2020/06/15 발표

#### 개요
* 개발자들을 위한 커뮤니티이며 회원제로 운영됩니다. <br>
  게시판과 질문게시판에서 활동 시 포인트를 부여하여 회원들의 활발한 참여를 독려합니다.
* 요약 : 개발자를 위한 커뮤니티 사이트, 추천사이트 제공, 개발자 고민, 개발자들의 꿀팁 공유

#### 공헌한 내용
* 참여도: **40%**
* 맡은 파트 : 회원가입, 로그인/로그아웃, 마이페이지(글수정, 파일업로드)
* 로그인 닉네임 중복체크 처리 : jQuery, Ajax, JSON, Gson lib
* 웹 화면 구성 : HTML, CSS, BootStrap, JavaScript
* 결과를 얻어오기 위한 서버 액션 : JAVA, Servlet, JSP, JSTL, EL
* DB액션 처리 : JDBC
* 사용기술: Java, JSP MVC model2, JSTL, EL, JDBC, Oracle 11g <br>
            Apache Tomcat9.0, HTML5, CSS3, jQuery, BootStrap, AJAX <br>
            CKEditor, JavaMail(mail.jar), JAF(activation.jar),  <br>
            gson/cos/jackson library

#### 사용 Tool
* ERD 설계와 DDL 작성: AQueryTool, DBeaver
* Flow Chart 작성: Draw.io
* 개발환경: Eclips, Apache Tomcat v9.0, Visual Studio Code, Oracle 11g
* 협업툴: GitHub

<br>
<br>
<br>


* * *
* * *

# 개인 프로젝트(Front) 1

* 프론트 UI 구현
* [이디야 메인홈페이지 벤치마킹 웹제작(유튜브 시연영상 바로가기)]   
(https://youtu.be/d7UjXUOFJWo)

#### 개요
* 카페 브랜드 EDIYA 메인 홈페이지를 벤치마킹하여 UI 구현

#### 공헌한 내용
* 공헌도: **100%**
* 웹화면 구성: HTML5, CSS
* 유효성 검증처리 : javaScript, jquery
* 개발 Tool: Eclipse, Visual Studio Code
<br>
<br>
<br>


* * *
* * *

# 개인 프로젝트(앱기획서) 2

* 무료나눔앱 화면기획서 작성 (첨부파일 참고)   

#### 개요
* 철 지난 아이용품을 무료로 나눔할 수 있는 공간
* 아이를 가진 부모들의 정보공유 및 일상 이야기를 할 수 있는 공간   

#### 공헌한 내용
* 공헌도: **40%**
* 맡은 역할: 프로젝트 기획, 화면기획서 작성
* 기획서 작성: MS Office(PowerPoint)
* 화면 프로토타입 연결: Adobe XD
<br>
<br>
<br>

* * *
* * *

# 코리아IT아카데미 JAVA 프로그래밍 교육 이수

#### 이수 과정명
* JAVA 프로그래밍 과정   

#### 교육 기간
* 2020.01.14 ~ 2020.03.24 (일 2시간, 총 80시간)   

#### 교육 내용
* 1주차: JAVA 기본구조, 데이터 타입, 기본 출력   
* 2주차: Scanner, 연산자, 제어문   
* 3주차: 배열, 클래스와 객체, 메서드   
* 4주차: 상속, 추상클래스, 인터페이스   
* 5주차: 예외처리, java.lang 패키지   
* 6주차: inner class, Collection 인터페이스   
* 7주차: java.util 패키지, 쓰레드   
* 8주차: java.io 패키지, GUI 프로그래밍

<br>
<br>
<br>

* * *
* * *

# 코리아IT아카데미 Python 프로그래밍 교육 이수

#### 이수 과정명
* Python 프로그래밍 과정   

#### 교육 기간
* 2020.01.18 ~ 2020.02.16 (주 2시간, 총 32시간)   

#### 교육 내용
* 1주차: 파이썬 기본 구조 및 자료형, 숫자형   
* 2주차: 문자열 자료형, 리스트, 튜플   
* 3주차: 딕셔너리, 셋, 불리언, 변수, 제어문1(조건문 if)   
* 4주차: 반복문 while, for, 함수 개념   
* 5주차: 함수 만들기 및 응용, 사용자 입출력, 파일 입출력   
* 6주차: 클래스 개념   
* 7주차: 모듈, 패키지   
* 8주차: 예외처리, 종합 문제 풀이   

<br>
<br>
<br>

* * *
* * *

# 코리아IT아카데미 국비지원과정 교육이수 중

#### 이수 과정명
* Java 프레임웍기반 풀스택 양성

#### 교육 기간
* 2020.03.16 ~ 2020.08.06 (일 8시간, 총 776시간, 97일)

#### 교육 내용
- **프로그래밍 언어활용 - JAVA (120시간)**<br>
  기본문법, 객체지향 프로그래밍, 다형성, Collection, Exception, Inner class, Stream
  
- **데이터베이스 구현 및 SQL - Oracle (40시간)**<br>
  DML, DDL, DCL, 단일행/그룹함수, Join, SubQuery, View   
 JDBC, 트랜잭션 처리
  
- **Android (50시간)**<br>
 뷰, 위젯, 이벤트 핸들링, 액티비티,   
 Handler, Storage   
 위치기반앱, 구글맵, 플레이스토어 
  
- **Web FrontEnd (110시간)**   
  HTML 5 / CSS3 / JavaScript / jQuery   
 반응형웹 / BootStrap / AJAX   
 JSON / XML / 각종 API   
  
- **JSP 기반 웹 프로그래밍 (100시간)**<br>
  Servlet / JSP / JSTL / EL /   
 쿠키, 세션, 파일업로드   
 MVC model2 기반 웹 어플리케이션 구현   
 AJAX, API 서버 설계 및 구축   
 Jackson, COS 등 라이브러리 활용   
 CKEditor 연동   
 Tomcat 서버   
  
- **MVC모델2 기반 웹어플리케이션 제작 (80시간)**<br>
  
- **Spring Framework (100시간)**<br>
  Dependency Injection, Autowire, DI Config   
 AOP, Sping MVC   
 request mapping, validation   
 Spring-jdbc, Transaction   
 ORM (MyBatis), Interceptor   
 REST, Secutiry   
  
- **디바이스  애플리케이션 구현 - Aduino (40시간)**<br>
  임베디드 애플리케이션 구현   
  
- **스프링 프레임워크 기반 웹어플리케이션 제작 (136시간)**<br>
