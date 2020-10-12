## 활용교재

- https://webskills.kr/2018/data/WEB_HTML_CSS.pdf

## 예제파일 링크

- https://repl.it/join/kgtzcjwc-junilhwang
- [메뉴 만들기](./example01.html)
- [슬라이드 만들기](./example02.html)

## 관련 링크

- [css-slide 만들기](http://junil-hwang.com/blog/css-slide-animation/)

## 복습

- display
  - `자기 자신`의 레이아웃을 변경
    - `inline`
      - 가로, 세로, 여백 지정 불가 (오작동)
      - 글자처럼 취급
    - `block`
      - 가로, 세로, 여백 지정 가능
      - 무조건 줄바꿈
    - `inline-block`
      - 가로, 세로, 여백 지정 가능
      - 글자처럼 취급
      - inline + block을 합친 속성
    - `none`
      - 요소가 안 보이도록 한다.
  - `자식 태그`의 레이아웃을 변경
    - flex
      - flex로 지정된 태그의 `자식 태그`를 가로로 정렬
      - 가로, 세로, 여백 지정 가능

## 선택자

- 모든 태그 선택은 `*`를 이용합니다.
  - `* { margin:0; padding: 0; }`
- 자식 선택은 `>`를 이용합니다.
  - `부모태그 > 자식태그`
- 자손 선택은 `스페이스바( )`를 이용합니다.
  - `조상태그 자식태그`
- `n`번째 태그 선택: `nth-child(n)`
  - `.slide-wrap > div:nth-child(1)`
  - `class="slide-wrap"`인 태그의 자식 중 첫 번째 div 태그

## padding, margin

- `padding: 10px`
  - 상,하,좌,우 10px
- `padding: 10px 15px`
  - 상,하 10px / 좌,우 15px
- `padding: 10px 15px 7px`
  - 상 10px / 하 7px / 좌,우 15px
- `padding: 10px 15px 7px 5px`
  - 상 10px / 우 15px / 하 7px / 좌 5px
- `margin: 10px`
  - 상,하,좌,우 10px
- `margin: 10px 15px`
  - 상,하 10px / 좌,우 15px
- `margin: 10px auto`
  - 상,하 10px / 좌,우 `(100% - width) / 2`
- `margin: 10px 15px 7px`
  - 상 10px / 하 7px / 좌,우 15px
- `margin: 10px 15px 7px 5px`
  - 상 10px / 우 15px / 하 7px / 좌 5px

## border

- `border`
  - 상하좌우 테두리에 대해서 사용 가능
- `border-top`
  - `상측` 테두리
- `border-bottom`
  - `하측` 테두리
- `border-left`
  - `좌측` 테두리
- `border-right`
  - `우측` 테두리
- `border-width`
  - `border-width: 1px` : 상하좌우 테두리의 너비를 1px
  - `border-width: 1px 2px` : `상하` 1px / `좌우` 2px
  - `border-width: 1px 2px 3px` : `상` 1px / `하` 2px / `좌우` 3px
  - `border-width: 1px 2px 3px 4px` : `상` 1px / `우` 2px / `하` 3px / `좌` 4px (시계방항)
- `border-style`
  - `border-style: solid` 직선
  - `border-style: dotted` 점선1
  - `border-style: dashed` 점선2

## display: flex
- `justify-content`
  - `justify-content: center` 자식 요소를 가운데 정렬 합니다.

## transition

- 변화를 서서히 일으킨다.
- `transition: 0.3s`
  - 0.3초 동안 변화가 일어난다.
  - 즉, 0.3초 동안 애니메이션이 발생한다.

## @keyframes
- keyframes을 통해서 애니메이션을 만들 수 있다.

```css
// slide01 이라는 애니메이션을 정의한다.
@keyframes slide01 {
  /*
    진행률 { 진행 시점에 대한 속성(Property)과 값(Value) }
  */
  0% { margin-left: 0 } /* 6초를 기준으로 0초 시점 */
  33% { margin-left: -1000px } /* 6초를 기준으로 2초 시점 */
  66% { margin-left: -2000px } /* 6초를 기준으로 4초 시점 */
  100% { margin-left: 0 }  /* 6초를 기준으로 6초 시점 */
}

div {
  /*
    animation: [애니메이션 이름] [애니메이션의 실행 시간] [반복횟수]
  */
  animation: slide01 6s infinite;
}
```

## overflow

- 사전적의미는 `넘쳐흐르다`라는 뜻
- 넘쳐흐르는 영역에 대한 제어
- `overflow: hidden` 넘쳐 흐르는 영역이 보이지 않도록 한다.
- `overflow: auto` 넘쳐 흐르는 영역이 있을 경우 스크롤이 생긴다.
- `overflow: visible` 무조건 스크롤이 생긴다. 