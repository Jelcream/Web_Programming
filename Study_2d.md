## 목록 태그
현대 웹 페이지에서 빠지지 않고 등장하는 요소가 있다면 내비게이션 메뉴임

내비게이션 메뉴는 웹 사이트의 다른 웹 페이지로 이동할 수 있는 버튼을 모아둔 것

#### 목록 태그
태그 | 설명
:--:|:--:
ul | 순서가 없는 목록<sub>unordered list</sub> 생성
ol | 순서가 있는 목록<sub>ordered list</sub> 생성
li | 목룍 요소<sub>list item</sub> 생성

<br><br>
## 테이블 태그
표를 만들 때는 테이블 태글 ㄹ사용

#### 테이블 태그
태그 | 설명
:--:|:--:
table | 표 삽입
tr | 표에 행<sub>table row</sub> 삽입
th | 표의 제목 셀<sub>table heading</sub> 생성
td | 표의 일반 셀<sub>table data</sub> 생성
<br>

1. 표 만들기
2. 셀 추가하기

+ thead, tbody 
    + thead, tbody는 테이블에서 콘텐츠들을 하나의 그룹으로 묶을 때 사용
    + 테이블의 각 영역(header, body, footer)을 명시하기 위해 사용
    + 브라우저는 이러한 요소들을 사용하여 테이블의 헤더나 푸터와는 독립적으로 테이블의 내용만 스크롤 되게 할 수 있으며, 여러 페이지에 걸쳐 있는 큰 테이블을 인쇄할 때 각 페이지의 상단과 하단에 테이블의 헤더와 푸터가 모두 인쇄되도록 할 수 있음
    + 기본적으로 웹 페이지의 레이아웃에 전혀 영향을 주지 않지만, 이 요소들의 스타일을 CSS를 사용하여 변경할 수는 있음
    + thead 요소는 table의 요소로써, 반드시 &lt;caption&gt;, &lt;colgroup&gt; 요소 다음에 위치해야 함
    + 반드시 하나 이상의 &lt;tr&gt; 요소를 포함하고 있어야함

<table border="1">
    <tr><th colspan="3">테이블 태그의 속성</th></tr>
    <tr>
        <th>태그</th>
        <th>속성</th>
        <th>설명</th>
    </tr>
    <tr>
        <th>table</th>
        <th>border</th>
        <th>표의 테두리 두께 지정</th>
    </tr>
    <tr>
        <th rowspan="2">th,td </th>
        <td>colspan</td><td>셀의 너비 지정</td>
    </tr>
    <tr><td>rowspan</td><td>셀의 높이 지정</td></tr>
</table>
<br>

[table tag reference](http://tcpschool.com/html-tags/thead)
<br><br>

## 미디어 태그
+ 이미지를 삽입할 때 img 태그를 사용
+ 음악을 삽입할 때 audio 태그를 사용(HTML5에 추가된 기능 이므로 인터넷 익스플로러 8 이하에서는 사용할 수 없음)

<br>

#### 미디어 태그 구분
내용물을 가질 수 있는 태그| 내용물을 가질 수 없는 태그
:--:|:--:
`<audio></audio>`<br>`<video></video>`|`<img>`


<br>

<table border="1">
    <tr><th colspan="3">이미지, 오디오, 비디오 태그의 속성</tr>
    <tr>
        <th>태그</th>
        <th>속성</th>
        <th>설명</th>
    <tr>
    <tr>
        <th rowspan="4">img 태그</th>
        <td>src</td>
        <td>이미지의 경로 지정</td>
    </tr>
    <tr>
        <td>alt</td>
        <td>이미지가 없을 때 나오는 글자 지정</td>
    </tr>
    <tr>
        <td>width</td>
        <td>이미지의 너비 지정</td>
    </tr>
    <tr>
        <td>height</td>
        <td>이미지의 높이 지정</td>
    <tr>
    <tr>
        <th rowspan="5">audio, video 태그</th>
        <td>src</td>
        <td>음악, 비디오 파일의 경로 지정</td>
    </tr>
    <tr>
        <td>preload</td>
        <td>음악, 비디오를 준비 중일 때 데이터를 모두 불러올지 여부 저장</td>
    </tr>
    <tr>
        <td>autoplay</td>
        <td>음악, 비디오의 자동 재생 여부 지정</td>
    </tr>
    <tr>   
        <td>loop</td>
        <td>음악, 비디오의 반복 여부 지정</td>
    </tr>
    <tr>
        <td>controls</td>
        <td>음악, 비디오 재생 도구 출력 여부 지정</td>
    </tr>
    <tr>
        <th rowspan="2">video 태그</th>
        <td>width</td>
        <td>비디오의 너비 지정</td>
    </tr>
    <tr>
        <td>height</td>
        <td>비디오의 높이 지정</td>
    </tr>
</table>

<br>

### 웹 브라우저 제약이 없도록 음악 삽입하기
+ 웹 브라우저마다 지원하는 확장자 형식이 다름
+ 게임기와 텔레비전에 들어가는 웹 브라우저 모두 지원하는 확장자가 다름
+ **웹 브라우저마다 음악 파일 확장자가 다른 문제는 source 태그로 해결이 가능**
+ source 태그는 audio 태그나 video 태그 내부에 입력함
+ HTML 페이지와 같은 폴더에 확장자가  OGG인 파일을 넣어 줌
+ 파일 변환 프로그램을 사용해도 되고 준비 파일을 사용해도 됨
<br>

### Source 태그
+ source 태그는 audio 요소나 video 요소, picture 요소에서 사용할 수 있는 다중 미디어 자원(multiple media resources)을 정의할 때 사용
+ source 요소는 미디어 타입이나 코덱의 지원여부, 미디어 쿼리에 따라 브라우저가 선택할 수 있는 대체 비디오/오디오/이미지 파일을 명시할 수 있도록 해줌 
+ 두 개의 소스 파일과 오디오 플레이어. 브라우저는 지원이있는 파일 (있는 경우)를 선택
+ [참고](http://www.w3bai.com/ko/tags/tag_source.html)

<br>

### 동영상을 불러오는 동안 다른 이미지 보여주기
+ video 태그의 poster 속성을 사용해 동영상을 불러오는 동안 사용자에게 보여 줄 이미지를 지정할 수 있음
+ img 태그의 src 속성처럼 이미지 경로를 입력

<br>

### 참고 OGG 파일
+ Ogg(오그) 멀티미디어 컨테이너 포맷
+ 특허권으로 보호되지 앟는 오픈 표준 파일 형식으로 멀티미디어 비트스트림을 효율적으로 전송하고 처리할 수 있게 하기 위해 Xiph.Org 재단에서 개발
+ [참고](https://ko.wikipedia.org/wiki/Ogg)

<br>

## 입력 양식 태그
입력 양식은 사용자에게 정보를 입력받는 요소

### 입력 양식
+ form xormfh duddurdmf todtjd
+ 내부에 input 태그를 넣어 만듬
+ Chapter4\01의 form_test에서 제출 버튼을 누르면 지정된 방식으로 지정된 장소에 데이터를 전달함
+ 이러한 전달 방식과 장소는 속성으로 지정
+ form 태그는 method 속성의 방식으로 action 속성 장소에 데이터를 전달함

```html
<form action="전송 위치" method="전송 방식">
</form>
```
+ 전송 위치

    데이터를 전달할 목적지
+ 전송 방식
    + GET: 주소에 데이터를 직접 입력해 전달
    + POST: 별도의 방법을 사용해 데이터를 해당 주소로 전달


### GET과 POST
URL에서 차이가 있음
예제에서 rint를 입력했다고 가정
+ GET 방식
    + 주소 창의 URL이 '파일 이름?search=rint'의 형태로 변경
    + GET 방식은 주소에 데이터를 입력해서 전달
    + 데이터 용량에 제한이 있음 (주소에 데이터를 입력하므로)

+ POST 방식
    + POST방식은 GET방식과 달리 비밀스럽게 데이터를 전달
    + 데이터를 별도로 전송하기 때문에 데이터 용량에 제한이 없음


<table border="1">
    <tr><th colspan="3">입력 양식 태그</th><tr>
    <tr>
        <th>태그</th>
        <th>속성</th>
        <th>설명</th>
    </tr>
    <tr>
        <th>form</th>
        <td>보이지 않음</td>
        <td>입력 양식의 시작과 끝 표시</td>
    </tr>
    <tr>
        <th rowspan="10">input</th>
        <td>text</td>
        <td>글자 입력 양식 생성</td>
    </tr>
    <tr>
        <td>button</td>
        <td>버튼 생성</td>
    </tr>
    <tr>
        <td>checkbox</td>
        <td>체크 박스 생성</td>
    </tr>
    <tr>
        <td>file</td>
        <td>파일 입력 양식 생성</td>
    </tr>
    <tr>
        <td>hidden</td>
        <td>해당 내용 표시 안 함</td>
    </tr>
    <tr>
        <td>image</td>
        <td>이미지 형태 생성</td>
    </tr>
    <tr>
        <td>password</td>
        <td>비밀번호 입력 양식 생성</td>
    </tr>
    <tr>
        <td>radio</td>
        <td>라디오 버튼 생성</td>
    </tr>
    <tr>
        <td>reset</td>
        <td>초기화 버튼 생성</td>
    </tr>
    <tr>
        <td>submit</td>
        <td>제출 버튼 생성</td>
    </tr>
    <tr>
        <td>textarea</td>
        <td>cols/rows</td>
        <td>여러 행의 글자 입력 양식 생성, cols는 너비를 지정하고 rows는 높이를 지정</td>
    </tr>
    <tr>
        <td>select optgroup option</td>
        <td></td>
        <td>선택 양식 생성<br>
        옵션 그룹화<br>
        옵션 생성</td>
    </tr>
    <tr>
        <td>fieldset legend</td>
        <td></td>
        <td>입력 양식의 그룹 지정<br>입력 양식 그룹의 이름 지정</td>
    </tr>
</table>

#### hidden 속성
+ 사용자가 입력하거나 선택하는 정보는 아닞지만 폼 전송이 같이 전송해줘야 하는 정보를 담기 위해서 히든 필드를 사용
+ 예: 사용자의 아이피 등
+ [참고][Reference]

[Reference]: http://www.homejjang.com/05/HiddenField.php

<br>

### label 태그
+ 이름, 생년월일, 성별처럼 input 태그를 설명할 때 사용
+ label 태그의 for 속성에 input 태그의 id속성을 입력해서 label 태그가 어떤 input태그를 나타내는지 알려주는 용도
+ for 속성을 연결하면, label 태그를 클릭했을 때 input 태그에 자동으로 포커스가 감
+ 체크 박스와 라디오 버튼 등은 레이블을 클릭했을 때 해당 항목이 체크됨