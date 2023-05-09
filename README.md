# js_bg_snow

★css
.body
background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%);
(ellipse)중심에서 (bottom)아래쪽 부터 시작해서 퍼져나가는것 

overflow: hidden;
웹 배경을 넘어가는 한이 있더라도 강제로 가려라

.snow
animation: snow 10s linear infinite;
10초동안 linear(균일한 속도) infinite(무한반복)

.snow:nth-of-type(2n)
animation-duration: 7s;
2의배수에 해당하는 눈은 7초

@keyframes snow
opacity 0은 안보이고 1은 잘보
snow 범위는 0에서 100vh 까지 transform
translate는 X,Y 전부 translate Y는 Y 좌표만

★js
createSnow 메소드
snow element 추가 
랜덤포지션

루프
createSnow 루프
