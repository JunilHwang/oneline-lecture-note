## 활용교재

- https://webskills.kr/2018/data/WEB_HTML_CSS.pdf

## 예제파일 링크

- https://repl.it/join/kgtzcjwc-junilhwang

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
- `margin: 10px 15px 7px`
  - 상 10px / 하 7px / 좌,우 15px
- `margin: 10px 15px 7px 5px`
  - 상 10px / 우 15px / 하 7px / 좌 5px