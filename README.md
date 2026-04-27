
aref=""
img src="images/a1.jpeg"

href="https://lol.ps/"target="_blank"

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 2주차 수업 내용
실습 1 : 트렌드/이론 분석
실습 2 : 실습: Quarkus 개발 환경 구축
실습 3 : 실습: LOL 메인 화면 페이지 만들기
실습 4 : 응용: LOL 메인 화면 페이지 만들기

## 2주차 수업 내용

Quarkus: 클라우드 네이티브 Java 프레임워크

Java 기반 백엔드 프레임워크: Quarkus는 클라우드 환경에 최적화된 Java 프레임워크입니다.
빠른 시작 시간과 낮은 메모리 사용이 특징입니다.
컨테이너 환경에서 실행에 최적화되어 있습니다.
GraalVM 네이티브 컴파일을 지원하여 성능을 극대화합니다.
컨테이너/Kubernetes, 서버리스 지원: 현대적인 클라우드 환경에 필수적인 기술들을 지원합니다.

장점: Spring Boot 대비 10배 빠른 부팅 속도와 AI 통합의 용이성.
단점: 빌드 시간이 길고, 기존 프로젝트를 Quarkus로 전환하기 어렵습니다.
클라우드 네이티브 컴퓨팅: 가상화 기술에서 발전하여 애플리케이션을 마이크로서비스로 분할하고, 자체 컨테이너에 패키징하며, 이를 동적으로 오케스트레이션하여 리소스 사용을 최적화하는 방식입니다.
ex) html 코드

<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quarkus Hello World</title>
</head>
<body>
    <div class="container">
        <h1>Hello, Quarkus!</h1>
        <p>이 파일은 <code>META-INF/resources/index.html</code>에서 실행 중입니다.</p>
    </div>
</body>
</html>

1단계: 기본 골격 및 태그 (문자열) 작성:
index.html 파일을 백업하고 새로 수정합니다.
h1, p, ul, li, div 등의 HTML 태그를 사용하여 LOL 메인 화면의 기본 구조를 잡습니다.
<!DOCTYPE html>: HTML5 문서 형식 선언 
<html>: HTML 문서의 최상위 컨테이너 
<head>: 브라우저에 표시되지 않는 메타데이터(문서 제목, 스타일 시트 등) 포함 
<meta>: 문자 인코딩, 뷰포트 등 정의 
<title>: 브라우저 상단 탭에 표시되는 문서 제목 설정 
<body>: 사용자에게 실제로 보이는 모든 콘텐츠 작성 
<div>: 특별한 의미 없이 요소를 그룹화하거나 레이아웃을 나누는 박스 모델 역할 (화면에는 표시되지 않음) 
<h1>: 문서 내에서 가장 중요한 제목을 정의 (글자가 크고 굵게 표시, 검색 엔진에 중요) 
<p>: 일반적인 텍스트 문단을 구분 (문단 앞뒤로 여백 생성) 
<ul>: 순서가 없는 목록 생성 (점/블릿 기호로 표시) 
<li>: <ul> 또는 <ol> 태그의 자식으로만 존재하며 목록의 개별 항목을 나타냄 
<code>: 프로그래밍 코드나 경로명을 나타낼 때 사용 (고정폭 글꼴로 렌더링)

2단계: Bootstrap 레이아웃 및 네비바 적용:
link, nav, div (상세 속성), img 등 태그를 사용하여 디자인을 적용합니다.
<link>: 외부 CSS 파일(Bootstrap 등)을 가져와 현재 문서에 적용합니다. <head> 안에 작성하며, href 속성으로 경로를 지정합니다. 
p.23
<nav>: 상단 메뉴나 링크 모음 구역임을 나타내는 의미론적 태그입니다. 웹사이트의 '길잡이' 역할을 하는 메뉴바를 만들 때 사용됩니다. 
p.23
container 클래스: 콘텐츠를 화면 중앙에 배치하고 좌우 여백을 자동으로 조절합니다. Bootstrap의 가장 기본 박스로, 내용이 화면 끝에 붙지 않게 합니다. 
p.23
row / col 클래스: 요소를 가로(row) 한 줄에 세우고, 칸(col)의 너비를 나눕니다. 한 줄을 12칸으로 나누어 배치하는 Bootstrap의 핵심 기술입니다. 
p.23
navbar-dark bg-dark: 네비바의 글자색을 밝게 설정하여 어두운 배경과 대비시킵니다. bg-dark와 함께 쓰여 검은색 상단 바를 만들 때 필수입니다. 
p.23
img (class 속성): card-img-top 등의 클래스를 통해 틀에 맞는 이미지 크기를 가집니다. 디자인 틀(카드 등)에 맞춰 이미지를 자동 정렬합니다. 
p.23
Div 영역은 여러 개의 영역이 중첩되어 표현됩니다. 
p.24

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 3주차 수업 내용
실습 1 : 트렌드/이론 분석
실습 2 : 실습: Quarkus 개발 환경 구축
실습 3 : 실습: LOL 메인 화면 페이지 만들기
실습 4 : 응용: LOL 메인 화면 페이지 만들기

## 3주차 수업 내용

3단계: 커스텀 스타일링 (LOL 테마 디자인):
<style> 태그를 사용하여 어두운 배경 및 포인트 컬러를 적용합니다.
<style> 태그는 <link> 태그 다음에 삽입하며, <h2> 태그에 클래스를 적용합니다. 

background-color: 웹 페이지나 특정 요소의 배경 색상을 지정합니다. #0a0e17 같은 헥사 코드를 사용하여 LOL 특유의 어두운 분위기를 만듭니다. 

color: 텍스트의 색상을 변경합니다. 배경이 어두워졌으므로 글자색을 #fff (흰색)로 설정하여 가독성을 확보합니다. 

font-family: 텍스트에 적용할 폰트 종류를 설정합니다. 사용자 컴퓨터에 설치된 폰트나 웹 폰트를 불러와 디자인 일관성을 유지합니다. 

linear-gradient: 두 가지 이상의 색상을 자연스럽게 섞어 배경에 입힙니다. 단순한 단색 배경보다 고급스럽고 입체적인 느낌을 줍니다. (배너 등에 활용) 

border: 요소의 가장자리에 선을 그립니다. border: none;을 사용하여 Bootstrap 기본 테두리를 제거하고 깔끔한 화면을 만듭니다.

accent-purple/red: 중요한 강조 사항에 사용할 보라색과 빨간색을 정의한 클래스입니다. 브랜드 아이덴티티를 나타내는 색상을 클래스로 만들어 반복 재사용합니다.

<h2 class="text-center accent-purple">챔피언 선택</h2>처럼 <style> 태그에 정의된 accent-purple 클래스를 <h2> 태그에 적용할 수 있습니다. 

4단계: 상호작용 및 디테일 (인터랙티브):
마우스 호버(Hover) 효과와 전환(Transition) 애니메이션 추가:
.card: transition: transform 0.3s, box-shadow 0.3s;를 추가하여 카드에 마우스를 올렸을 때 부드러운 변화를 줍니다. 

transition: 속성(크기, 색상 등)이 변할 때 부드럽게 바뀌는 시간을 설정합니다. 이것이 없으면 변화가 뚝뚝 끊깁니다. 

.card:hover: transform: scale(1.05); (마우스를 올리면 105% 커짐), box-shadow: 0 10px 20px rgba(160, 32, 240, 0.5); (보라색 광원 효과)를 추가하여 상호작용 효과를 줍니다. 

:hover: 사용자가 요소 위에 마우스를 올렸을 때만 스타일이 적용되도록 하는 가상 클래스입니다. 

transform: scale: 요소를 확대하거나 축소합니다. 특정 항목이 선택되었음을 시각적으로 강조할 때 효과적입니다. 

box-shadow: 요소 뒤에 그림자나 광원 효과를 추가합니다. rgba 값으로 보라색 투명도와 그림자 위치 등을 조절합니다. 

이미지 비율 최적화 (object-fit: cover):
.card-img-top: height: 200px; (세로 길이 고정), object-fit: cover; (이미지가 찌그러지지 않게 채움)를 추가하여 이미지 크기를 조정합니다. 
 

height: 요소의 세로 길이를 고정합니다. 여러 장의 이미지가 서로 다른 크기여도 카드 전체의 높이를 일정하게 맞춰줍니다. 

object-fit: cover: 이미지가 찌그러지지 않고 정해진 틀을 가득 채우도록 합니다. 이미지가 옆으로 퍼지거나 위아래로 찌그러지는 것을 방지하여 퀄리티를 높여줍니다.

# quarkus 프로젝트 시작! (학번 :20231034 이름 :허성욱 )
매 주 수업 내용을 정리하자.
## 4주차 수업 내용
실습 1 : 부트스트랩 5 이해/활용하기
실습 2 : 하이퍼 링크와 이미지
실습 3 : 네비게이션 바 수정하기
실습 4 : 카드 – 모달창 구현하기

## 4주차 수업 내용
"부트스트랩 5 이해/활용하기"
공식 웹 사이트: https://getbootstrap.kr/ 에서 최신 버전(5.3)의 문서와 디자인 샘플을 확인한다.
LOL 홈페이지 resources 폴더의 index.html 파일을 열어 <head> 태그 내에 CDN 방식으로 부트스트랩을 연동한다. CDN (Content Delivery Network)은 콘텐츠를 빠르게 전달하는 방식이다.
문서의 기본 정보
<head> 태그 안에 <meta>, <link>, <script> 등의 태그로 문서의 기본 정보를 포함한다.
<meta>: 페이지의 주요 전역 정보 (예: charset="UTF-8", viewport 설정).
<link>: 외부 자원 연결 (예: CSS 파일).
<script>: 자바스크립트 연결.
LOL 기본 메인 화면 살펴보기

HTML5와 부트스트랩 5 코드가 혼합되어 사용된다.
부트스트랩 5의 요소를 구분하기 위해 <nav> 태그와 class 속성들을 확인한다. navbar, navbar-expand-lg, navbar-dark 등의 클래스는 네비게이션 바의 디자인과 동작을 정의한다.

부트스트랩 5를 주석 처리하여 해제하면 화면이 어떻게 변하는지 확인하여 부트스트랩의 영향을 이해할 수 있다.
하이퍼 링크와 이미지
하이퍼 링크 (hyperlink)는 <a href="..."> 태그를 사용하여 페이지를 연결하며, href 속성에 링크 주소(URL)를 지정한다.
현재 LOL 링크 주소는 #으로 설정되어 있어 페이지 이동이 없으므로, 로컬 주소 (http://localhost:8080/)나 외부 웹사이트 주소 (https://www.leagueoflegends.com/ko-kr/)로 수정하여 페이지를 연결할 수 있다.
이미지는 <img src="..."> 태그를 사용하여 로딩하며, src 속성에 이미지 경로를 지정한다.
외부 URL에서 이미지를 로딩하거나, resources 폴더 안에 images 폴더를 생성하여 다운로드한 이미지를 로컬에서 로딩할 수 있다.
경로 지정 시 상대 경로 (../images/Aatrox.png)와 절대 경로 (/images/Aatrox.png)의 차이를 이해하고 사용한다.
웹 서버는 기본적으로 index.html 파일을 로딩하며, 잘못된 주소로 접속 시 404 에러 (Resource Not Found)가 발생한다. 
HTTP 상태 코드 (200, 301, 304, 400, 404, 500)의 의미를 이해하는 것이 중요하다.


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


## 5주차 수업 내용
<head> 태그 안에 <meta>, <link>, <script> 등의 태그로 문서의 기본 정보를 포함한다.
<meta>: 페이지의 주요 전역 정보 (예: charset="UTF-8", viewport 설정).-문자 인코딩,스마트폰 등 화질 
<link>: 외부 자원 연결 (예: CSS 파일).
<script>: 자바스크립트 연결.
하이퍼 링크 (hyperlink)는 <a href="..."> 태그를 사용하여 페이지를 연결하며, href 속성에 링크 주소(URL)를 지정한다.

현재 LOL 링크 주소는 #으로 설정되어 있어 페이지 이동이 없으므로, 로컬 주소 (http://localhost:8080/)나 외부 웹사이트 주소 (https://www.leagueoflegends.com/ko-kr/)로 수정하여 페이지를 연결할 수 있다.
이미지는 <img src="..."> 태그를 사용하여 로딩하며, src 속성에 이미지 경로를 지정한다.

외부 URL에서 이미지를 로딩하거나, resources 폴더 안에 images 폴더를 생성하여 다운로드한 이미지를 로컬에서 로딩할 수 있다.

경로 지정 시 상대 경로 (../images/Aatrox.png)와 절대 경로 (/images/Aatrox.png)의 차이를 이해하고 사용한다.

웹 서버는 기본적으로 index.html 파일을 로딩하며, 잘못된 주소로 접속 시 404 에러 (Resource Not Found)가 발생한다. HTTP 상태 코드 (200, 301, 304, 400, 404, 500)의 의미를 이해.

CSS 선택자 (Selector)의 관계와 우선순위를 이해하는 것이 중요하다.
기본 (요소) < 외부 (클래스) < 내부/인라인 (ID) 순으로 우선순위가 높아진다.
!important는 가장 높은 우선순위를 가진다. 

서브페이지 추가:
기존 <style> 태그 대신 <link rel="stylesheet" href="../css/download.css">를 사용하여 CSS 파일을 페이지에 연결한다.




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

## 7주차 과제 내용 


showMainScreen() 함수를 만든다
performSearch에서 q가 없으면 호출(조건)

function showMainScreen() {
    // 검색 결과 섹션 숨기기
    document.getElementById('searchResults').classList.add('d-none');
    document.getElementById('searchResults').style.display = 'none';

    // hero 섹션 다시 보이기
    document.querySelector('.hero').classList.remove('d-none');

    // 기존 section들 다시 보이기 (searchResults 제외한 모든 section)
    document.querySelectorAll('section:not(#searchResults)').forEach(s => s.classList.remove('d-none'));

    // 검색 입력창 초기화
    document.getElementById('searchInput').value = '';
}


검색어 입력(submit)
    ↓
performSearch(query) 호출
    ↓
q = query.trim().toLowerCase()
    ↓
q가 비었거나 공백? → showMainScreen() → return
    ↓ (검색어 있을 때)
검색 결과 렌더링 → section 숨김 → searchResults 표시


