# 웹 프로그래밍 입문 Book 공부

### HTML5 기본 용어
태그, 요소, 속성
+ HTML 페이지를 구성하는 각 부품을 **요소**라고 함
+ 태그는 이러한 요소를 만들 때 사용하는 작성 방법
+ 속성은 태그에 추가 정보를 부여할 때 사용하는 것
+ 요소와 태그를 구분하지 않고 사용하기도 함   

### 생성 방법에 따른 요소 구분
요소 구분 | 형태 | 예
|--|:--:|--:|
|내용을 가질 수 있는 요소| <요소 이름>내용</요소 이름> | `<h1>Hello html5</h1>`<br>`<p>즐거운 웹 프로그래밍 입문</p>`
|내용을 가질 수 없는 요소| <요소 이름> |`<img>`<br>`<br>`<br> `<hr>`

### 내용에 들어갈 수 있는 것

1. 텍스트
2. 다른 태그
3. 내용을 입력하지 않은 경우

### 속성
+ **__속성은 태그에 추가 정보를 부여할 때 사용하는 것__**   
    `<h1 title="header">header</h1>`
+ title 은 속성 이름, "header"은 속성 값   

### 주석
+ `<!--주석-->`

## HTML5의 구조
```html
<!DOCTYPE html>
<html> <!-- 모든 HTML 페이지의 기본 요소로, 모든 태그는 이 html태그 내부에 작성함 -->
    <head><!-- Body 태그에 피룡한 스타일시트와 자바스크립트를 제공함 -->
        <title>Hello HTML5</title>
    </head>
    <body>
        <!-- 사용자에게 실제로 보이는 부분을 작성하는 곳 -->
    </body>
</html>
```
### html 태그의 lang 속성
lang 속성 값| 언어
|:--:|:--:|:--:|
ko|한국어
en|영어
ja|일본어
ru|러시아어
zh|중국어
de|독일어

### head 태그 내부에 넣을 수 있는 태그
태그| 설명
|:--:|:--:|:--:|
meta| 웹 페이지에 추가 정보 전달
title| 페이지 제목 지정
script| 웹 페이지에 스크립트 추가
link| 웹 페이지에 다른 파일 추가
style| 웹 페이지에 스타일시트 추가
base| 웹 페이지의 기본 경로 지정

## 스타일시트 작성과 실행
두 가지 방법의 스타일시트를 사용해 스타일을 적용   
HTMLPageWithStyle
1. HTML 페이지 내부에서 `style 태그`를 사용해 스타일시트를 직접 입력하는 `내부 스타일 방법`
2. 스타일시트를 별도의 파일로 만든 후, HTML 페이지 내부에서 link 태그의 `href(hyper reference) 속성`을 사용해 스타일시트를 불러오는 `외부 스타일 방법`
3. link rel="stylesheet" href="file.css"

## 자바스크립트 작성과 실행
두 가지 방법의 스타일시트를 사용해 스타일을 적용   
HTMLPAgeWithScript
1. `script 태그`를 사용해 내부에서 작성
2. `script 태그`의 `src 속성`을 사용해 외부에서 불러오도록 작성
3. 추가적으로 더 있으나, 1과 2가 기본적인 방법임

## 오류 및 검증
크롬 실행 후 f12 or ctrl + shif + i 누르면 검사 실행   
검사 기능은 다양하게 있으며 도느 엡 페이지를 대상으로 검사를 실행할 수 있음
+ `[Elements]`탭에서는 현재 HTML 페이지의 계층 구조와 각 태그에 적용된 스타일을 파악할 수 있음
+ `[Console]`탭은 오류를 확인하거나 자바스크립트 코드를 추가로 입력할 때 사용
  + 오류가 발생하면 원인과 위치를 알려줌


## 글자 태그
글자 태그는 종류가 매우 다양함
+ 제목과 본문 글자 태그
  + `h` : `heading(제목)`
  + `p` : `paragraph(단락)`
  + `br` : `breadk(줄바꿈)`
  + `hr` : `horizontal rule(수평 줄)`
    태그 | |설명
    |:--:|:--:|:--:|
    제목 글자|h1<br>h2<br>h3<br>h4<br>h5<br>h6|첫 번째로 큰 제목 글자 생성<br>두 번째로 큰 제목 글자 생성<br>세 번째로 큰 제목 글자 생성<br>네 번째로 큰 제목 글자 생성<br>다섯 번째로 큰 제목 글자 생성<br>여섯 번째로 큰 제목 글자 생성<br>|
    본문 글자|p<br>br<br>hr<br>|본문 문단 생성<br>줄 바꿈<br>수평 줄 삽입|
    
    ## 특수 문자 표기
    공백, 괄호 등은 다음 특수 문자를 사용해 화면에 표시할 수 있습니다.
    특수 문자|출력 문자
    |:--:|:--:|:--:|
    `&nbsp;`(non-breaking space) | 공백
    `&lt;`(less than) | <
    `&gt;`(greater than) | >
    `&amp;`(ampersand)| &
    `&quot;`|"

    + html 태그 내부에 `공백 3개`를 연속으로 입력한 후 파일을 실행하면 `연속된 공백을 1개로 인식`하기에 공백 3개가 제대로 표시되지 않는다.

## 앵커 태그
HTML<sub>HyperText Markup Language</sub> 에서 중요한 글자는 H<sub>HyperText</sub>임

하이퍼텍스트는 사용자 선택에 따라 관련한 특정 정보로 이동할 수 있도록 조직된 문서를 의미

이러한 조직된 문서 형태는 a태그의 지분이 큼   
<br>
### a 태그 Anchor
태그|설명
|:--:|:--:|
a|하이퍼링크 생성
+ a 태그만으로는 어떤 웹 페이지로 이동할지 웹 브라우저에 알려 줄 수 없음
+ `href`<sub>`Hyper Reference`</sub> 속성을 사용하여 웹 페이지나 파일의 위치를 나타내는 경로를 입력
+ `<a href="https://naver.com">네이버</a>`
+ 태그 사이에 있는 내용은 출력 글자임
+ 새로운 창에서 열게 할 때는 target="_blank"를 줄 것

<br>

### 웹 페이지 내부에 연결하기
웹 페이지 내부의 특정 태그로 이동하려면 id 속성을 추가로 사용
+ <태그 id="#id 속성">
+ href에 #id 속성을 넣으면 해당 내용으로 이동함
+ id속성이 중복되면 먼저 나오는 태그로 이동
  
### 빈 링크
a 태그의 하이퍼링크 기능을 제거하고 사용할 때도 있음   
하이퍼링크 기능을 제거하더라도 a 태그에 href 속성은 반드시 입력해서 웹 표준을 따라야 함
+ 웹 표준을 지키면서 이동하지 않는 a 태그   
    `href="#"`
+ 이를 `빈 링크`라고 함


<br>

[마크다운 문법 참조][first_reference]  

[first_reference]: https://gist.github.com/ihoneymon/652be052a0727ad59601   

[마크다운 문법 참조2](https://heropy.blog/2017/09/30/markdown/)

[마크다운 문법 참조3][third_reference]

[HTML Reference][HTML Reference W3c]

[HTML Reference W3c]: https://www.w3schools.com/html/default.asp

[third_reference]: https://inasie.github.io/it%EC%9D%BC%EB%B0%98/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%ED%91%9C-%EB%A7%8C%EB%93%A4%EA%B8%B0/
