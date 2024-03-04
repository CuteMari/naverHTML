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
