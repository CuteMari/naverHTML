## 1. inline, inline-block, block의 차이점
1) inline: width, heigth 없음
2) inline-block: width, height 존재 but block처럼 한 줄을 다 차지하지 않는다.
3) block: 한 라인을 모두 점유

## 2. id -> 태그를 구별하기 위해 사용
연관성있게 작명하는것이 중요

## 3. shortcut icon

## 4. 개발자 도구를 이용하여 이미지 다운받기
1. 서버에서 이미지 다운받기<br>   ex) \<link rel="shortcut icon" type="image/x-icon" href="/favicon.ico?1"><br>  -> https://www.naver.com/favicon.ico<br>  -> 네이버 서버에 있는 이미지를 다운받을 수 있다!<br>
2. css의 background-image<br>
  background-image: url(https://pm.pstatic.net/resources/asset/sp_main.ae81c9d5.png);

## 5. 필요에 따라 부모태그 혹은 자식태그를 추가로 넣어야 좋은 경우도 있다.
----------------------------------------------------------------
## 6. css코드에서 변수 사용 가능!
외우지 않고 변수를 활용하여 코드 작성 가능<br>
- 변수에 해당하는 값을 바꾸면 그 변수를 사용하는 곳은 전부 한 번에 바뀌어서 편리하다!
## 7. 박스 사이즈 box-sizing
요소의 전체 너비와 높이를 어떻게 계산하는지 설정한다.
1. content-box : 기본으로 설정되는 스타일
- 할당된 너비와 높이는 내용물(content)에만 적용된다.<br>
- border 혹은 padding을 추가하면 요소의 크기는 그만큼 더 커진다<br>
2. border-box
- border와 padding은 너비와 높이 값에 포함된다.
- 요소의 사이즈를 맞추는 것이 더욱 편리하기 때문에 **border-box를 선호**
## 8. padding vs margin
- padding: 요소에 포함된다
- margin: 요소에 포함 안됨
## 9. cursor:pointer
마우스를 올리면 손가락 모양이 나옴
## 10. position
요소가 어디에 있어야 하는지 조절하는 css
기본값: static
1. position: relative
- 자신의 static 위치를 기준으로 움직인다.
- top, right, bottom, left 속성을 자기 자신을 기준으로 적용
2. position: absolute
- 자신의 static 위치에서 완전히 벗어날 수 있다.
- **static이 아닌 속성이 부여된 부모를 기준**으로 위치를 설정한다. (기본은 \<body>)
3. position: fixed
- 스크롤을 내려도 같은 위치에 계속 있음
4. position: sticky
- 스크롤 하지 않을 때는 staic처럼 동작, 스크롤하면 fixed처럼 작동
-------------------------------------------
## 11. <a> <button> 
=> 클릭 가능한 요소
구분: a태그는 다른 페이지로 이동할 때 보통 사용한다. 버튼은 클릭 효과

## 12. placeholder

## 13. inline-block의 단점 => 요소들끼리 여백이 생길 수 있음
=> flex를 사용하면 좋다<br>
=> align-items, justify-content등.. 크롬 개발자 도구에서 미리보기 가능

-----------------------------------------------------------
## 14. focus-within
: 자식태그 중 focus된 태그가 있으면 활성화된다.

## 15. 리스트를 id 없이도 사용하는 방법
- ex) nav li:nth-child(번호){}
- ex) nav li:nth-of-type(번호){}<br>
nth-child보다는 **nth-of-tpye**를 추천!<br>
 => child는 만약 종류가 다른 태그가 들어있다면 그 태그도 순서에 포함될 수 있음 (중간 형제 태그를 모두 카운트한다) => 서로 다른 **태그를 구분하지 않음**<br>
 => of-type은 정한 태그의 종류만 카운트한다 => **태그를 구분함**
-------------------------------------------------------------------
## 16. aside[id$=ad]{}
: aside 중 id가 ad로 끝나는 요소를 한번에 담을 수 있음

## 17. section[id^=main]{}
: section요소 중 id가 main으로 시작하는 요소

## 18. grid
: 형제태그들이 알아서 **격자**모양으로 배치된다.
1. grid-template-rows: repeat(칸 수, 간격)
2. grid-template-columns: repeat(칸 수, 간격)
3. fr: 전체 너비/높이 중 차지할 비율
4. 크롬에서 grid도구 사용 가능
5. gird gap: grid안에 내부 경계선을 넣음
 - grid 요소들 사이의 gap을 설정한다
 - grid의 내부 색상을 바꾸고
 - gird 요소들의 내부 색상 또한 바꿔주면 됨
----------------------------
## 19. transform skewX()/skewY()
: 요소의 모양을 기울이거나 비틀 수 있음

## 20. 태그 속성 선택자

## 21. 한 줄에 나타나는 텍스트가 너비를 초과할 때 ...으로 표현하는 방법
1. text-overflow: ellipsis; <br>
2. text-overflow: hidden; => 너비를 넘어가는 부분은 ...으로 나옴<br>
3. white-space: nowrap; => 텍스트가 접히지 않는다 => 한 줄로만 표현됨

## 22. 빈 공간을 없앨 때에는 부모 요소를 flex로 바꿔주자
---------------
## 23. \&nbsp;
: html ntt(특수문자) 띄어쓰기

## 24. 요소 회전 transform: rotate()

## 25. css우선순위
1. 밑에 있을 수록 우선순위가 높다
2. id가 class보다 우선순위가 높다
3. 붙인 id/class가 많을 수록
등...<br>
3. important를 붙이면 우선순위가 가장 높아진다 ( 뒤에 !important ) => 최후의 수단으로 쓰는게 좋다













