## 활용교재

- https://webskills.kr/2018/data/WEB_HTML_CSS.pdf

## 예제파일 링크

- https://repl.it/join/kgtzcjwc-junilhwang

## HTML 이란?

- HyperText Markup Language
- 어떠한 정보를 의미하는 텍스트에 마크업(태깅)을 하여 문서를 만드는 언어
- 각각의 태그에는 특정 역할이 존재한다.
  - 제목 _(h1 ~ h6)_
  - 목록 _(ul, ol, li)_
  - 문단 _(p)_
  - 메뉴 _(nav)_
  - 링크 _(a)_
  - 사진 _(img)_

## CSS 

- 태그를 꾸미기 위한 도구
- 가로너비, 세로너비, 여백, 글자색, 배경색, 테두리, 그림자 같은 효과를 줄 수 있다.
- 애니메이션을 표현할 수 있다.
- 굉장히 많은 속성과 규칙이 존재하기 때문에 많은 경험이 필요하다.

## CSS Property

- width: 가로너비
- height: 세로너비
- color: 글자색
- background: 배경색
- font-size: 글자크기
- border: 테두리
- margin: 바깥여백
- padding: 안쪽여백
- line-height: 줄간격

## 간단한 Style 표현

```html
    <div style="width: 100px; background: #000; color: #fff; height: 100px; font-size: 20px; border: 10px solid #f00;">
      여백 없음
    </div>
    <div style="width: 100px; background: #000; color: #fff; height: 100px; font-size: 20px; border: 10px solid #f00; margin: 20px;">
      Margin 20px
    </div>
    <div style="width: 100px; background: #000; color: #fff; height: 100px; font-size: 20px; border: 10px solid #f00; padding: 20px; line-height: 200%">
      Padding 20px
    </div>
```

## class와 id

- id
  - 한 페이지에 한 개의 아이디만 존재 해야 한다.
  - 한 개의 태그에 대해 독립적으로 사용하기 위한 속성이다.
  - style에서 사용할 때 앞에 `#`을 붙인다.
  - 사용방법
```html
<style>
  #header {}
  #section {}
  #footer {}
</style>

<div id="header"></div>
<div id="section"></div>
<div id="footer"></div>
```

- class
  - 한 페이지에 여러 개의 class가 존재할 수 있다.
  - 여러 태그에 사용하기 위한 속성이다.
  - class 속성에 여러 개의 class를 정의할 수 있다.
  - style에서 사용할 때 앞에 `.`을 붙인다.
  - 사용방법
  
```html
<style>
  .center { text-align: center; }
  .red { color: red; }
  .blue { color: blue; }
  .size20 { font-size: 20px; }
</style>

<div class="center red">빨간 글자에 가운데 정렬</div>
<strong class="blue">파란 글자</strong>
<strong class="red size20">빨간 글자에 20px의 크기</strong>
<strong class="blue size20">파란 글자에 20px의 크기</strong>
```

## 위치를 변경하기 위한 속성

- display
  - display: block
    - 가로 너비, 세로 너비, 여백 등을 지정할 수 있다.
    - 기본적으로 가로너비는 100% 이다.
  - display: inline
    - 가로 너비, 세로 너비, 여백 등을 지정할 수 없다.
    - 글자 취급을 하는 속성이다.
  - display: inline-block
    - block과 inline의 특성을 합한 것
    - 가로 너비, 세로 너비, 여백 등을 지정할 수 있다.
    - 기본적으로 가로너비는 100%가 아니다.
    - 글자 처럼 취급 받는 속성이다.
  - display: flex
    - flex로 지정한 태그의 `자식` 태그를 가로로 정렬시킨다.
    - `기본(default)`가 가로정렬이고, 세로 정렬도 가능하다.
    
- float
  - float: left
  - float: right