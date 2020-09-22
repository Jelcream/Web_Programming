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
<br>

[마크다운 문법 참조][first_reference]  

[first_reference]: https://gist.github.com/ihoneymon/652be052a0727ad59601   

[마크다운 문법 참조2](https://heropy.blog/2017/09/30/markdown/)

[마크다운 문법 참조3][third_reference]

[third_reference]: https://inasie.github.io/it%EC%9D%BC%EB%B0%98/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%ED%91%9C-%EB%A7%8C%EB%93%A4%EA%B8%B0/
