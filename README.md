
aref=""
img src="images/a1.jpeg"

href="https://lol.ps/"target="_blank"

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 4주차 수업 내용
실습 1 : 부트스트랩 5 이해/활용하기
실습 2 : 하이퍼 링크와 이미지
실습 3 : 네비게이션 바 수정하기
실습 4 : 카드 – 모달창 구현하기

<div align="center">
<img src="screenshots/2026-01-26 오전 9_51_43.png" width="45%" alt="실습 1 화면">
<img src="screenshots/파일명.png" width="45%" alt="실습 2 화면">
</div>
<br>

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 5주차 수업 내용
실습 1 :  서브 페이지 추가하기
실습 2 : 서브 페이지 구현하기
실습 3 : 다운로드 페이지 구현
실습 4 : 다운로드 페이지 배경화면 및 시스템 사양 화면 구현 

<div align="center">
<img src="screenshots/2026-04-01 오후 141518.png" width="45%" alt="실습 5 화면">
<img src="images/down.jpg" width="45%" alt="실습 5 화면">
</div>
<br>


## x주차 수업 내용
테스트

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 6주차 수업 내용
실습 1 :  자바스크립트 개요
실습 2 :  자바스크립트 활용하기(부트5:외부)
실습 3 : 자바스크립트 기본 문법
실습 4 : 실시간 챔피언 검색하기 - 1


<div align="center">
<img src="화면 캡쳐 2026-04-18 142333.png" width="45%" alt="실습 4 화면">
<img src="" width="45%" alt="실습 4 화면">
</div>
<br>


## 6주차 수업 내용
자바스크립트: 
text 박스가 있는 창은 대부분이 form 형식이다. 

(ex)
<!-- <form class="d-flex" id="searchForm">
<input class="form-control me-2" type="search" placeholder="챔피언, 뉴스 검색..." aria-label="Search" id="searchInput">
<button class="btn btn-outline-success" type="submit">검색하기</button>
</form> -->

id는 고유 값 해당 form을 식별하기 위한 수단 
위에서 "searchForm" 라고 이름을 지정. 폼(inform)태크로 정의하며 식별자는 searchInput 

DOM(Document Object Model)이란?
• 왜 이런 것이 필요한가?
• HTML 로딩을 위한 표준 구조
• 트리 구조(DOM)로 변환하여 관리
• 문서의 구조화된 표현을 제공
• HTML 문서의 태그는 계층구조
• DOM의 트리 구조
• 최상위 객체 : Document로 정의
• JS, Python 등 언어에 독립적
• 자바스크립트로 무엇을 하는가?
• HTML 문서 구조, 스타일, 내용 등을 변경

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 7주차 수업 내용
실습 1 :   실시간 챔피언 검색하기 - 2 (디자인(스타일) 파일로 분리하기) 메인화면 소스코드에 <style>확인
및 자바스크립트와 같이 분리하여 관리하기 - <link rel="stylesheet" href="css/main.css">  
실습 2 : 메인화면 index.html 수정하기 
실습 3 : search.js 자바스크립트 수정하기 
• 데이터 타입 및 변수 정의
• 챔피온과 뉴스 데이터(객체 배열)
실습 4 : 실시간 챔피언 검색하기 - 2 
• 창을 유지, 하단 검색 결과 출력
• 아트록스 검색, 카테고리 클릭


<div align="center">
<img src="화면 캡처 2026-04-15 133215" width="45%" alt="실습 3 화면">
<img src="" width="45%" alt="실습 3 화면">
</div>
<br>


## 7주차 수업 내용

• 기본 동작(코드) 이해하기
• 현재 폼의 id는? searchForm (동일)
• 핵심 함수 : performSearch
• 데이터 셋으로 부터 : filter(조건 충족)
• 키워드 가운데 출력 : searchKeywordDisplay
• 필터 결과 카운팅(숫자), 0개인 경우 화면 처리
• 탭(기본) 전환 : switchCategory
• 카테고리 클릭(빨간 왼쪽 테두리), Type으로 판단
• 기존 섹션 숨김 : display: none
• 두 콘텐츠 하나만 표시 : 3항 연산자

• 동작 과정 그림 요약
• PART 1 : 사용자가 검색어를 입력하고 'Enter'를 누른 직후, 콜스택(Call Stack)에서 performSearch을 불러온다. 데이터 필터링 후 addEventListener을 등록

• PART 2 : js가 HTML 구조를 동적으로 생성하고, CSS를 조작하여 화면을 전환


