# CSS3 기초: 선택자와 단위


## 선택자
CSS3에서 특정 HTML 태그를 선택할 때는 선택자를 사용
+ 구조<br>
  선택자 { 스타일 속성: 스타일 값;}<br>
  h1 { color: red; }<br>
+ 자바스크립트에서도 사용 (??)
```html
<head>
<style>
    h1{
        color:red;
        background-color: orange;
    }
</style>
</head>

```
이 코드는 h1 태그의 color 스타일 속성에 스타일 값으로 red를 지정한다. 라는 것을 알 수 있음

[선택자 종류 참고1][1]

[선택자 종류 참고2][2]

[선택자 종류 참고3][3]

<br>

### 선택자 종류 
14개 너무 많은 거 아닌가?
+ 전체 선택자
+ 태그 선택자
+ 아이디 선택자
+ 클래스 선택자
+ 속성 선택자
+ 후손 선택자
+ 자손 선택자
+ 반응 선택자
+ 상태 선택자
+ 구조 선택자
+ 동위 선택자
+ 링크 선택자
+ 문자 선택자
+ 부정 선택자

### 콜론 개수의 따른 구분
1. **1개인 경우** : 가상 클래스<sub>pseudo-class selector</sub>  선택자
2. **2개인 경우** :: 가상 요소<sub>pseudo-element selector</sub> 선택자


## 기본 선택자
종류| 형태|설명
:--:|:--:|:--
전체 선택자|*|HTML 페이지 내부의 태그를 모두 선택
태그 선택자|태그|HTML 페이지 내부의 특정 태그를 모두 선택
아이디 선택자|#아이디|특정 id 속성이 있는 태그를 선택, 웹 표준에 id 속성은 웹 페이지 내부에서 중복되면 안 된다는 규정이 있어 아이디 선택자는 특정 태그 하나를 선택할 때 사용
클래스 선택자|.클래스|특정 클래스가 있는 태그 선택


[1]:http://www.nextree.co.kr/p8468/
[2]:https://aboooks.tistory.com/249
[3]:https://ssungkang.tistory.com/entry/css-css-%EC%84%A0%ED%83%9D%EC%9E%90selector-%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%EC%98%88%EC%8B%9C



[마크다운 참조][markdown_Reference]

[markdown_Reference]:https://simhyejin.github.io/2016/06/30/Markdown-syntax/#collapsible