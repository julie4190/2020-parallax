HTML 정리
block: 부모의 크기에 꽉 차게 영역을 차지한다(layout 잡을 때, 내용을 감쌀 때)
div: 특징이 없다.
h1~h6: 제목을 나타낼 때 쓴다. (font-weight: bold, padding, margin을 가진다)
p: 내용을 나타낼 때 쓴다. (margin-bottom을 가진다)
ul, li, dl, dd, dt: 목록을 나타낼 때 쓴다.
form, table
Normalize: block요소는 속성을 가지고 있기 때문에 초기화 하여 필요할 때 속성을 부여해서 쓴다
html, body, div, ul, li, dl, dd, dt, p, h1, h2, h3, h4, h5, h6, form, input, select, textarea, header, footer, section, article, aside, table, thead, tbody, tr, td, th {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-weight: normal;
}
inline: 글자요소(한줄에 나타남, 내용자체)
span: 글 안에서 영역을 설정할 때
a: 링크[href="#" target="_self(기본), _blank(새창), myName(프레임이름)"]
i: 이탤릭을 표시 - css의 font-style: italic;과 같다.
b, strong: 볼드를 표시 - css의 font-weight: bold;와 같다.
img: 이미지를 나타낸다[src="../img/p.jpg"], 이미지도 영문글자와 같이 취급되어 기준선이 baseline으로 잡혀서 하단으로 기준선을 아래와 같이 변경하여야 한다.
input, select, textarea 등등의 form요소
inline과 inline-block의 차이점은 width, height의 유, 무 차이.
inline: span, i, b, strong
inline-block: img, input, select, textarea
/* img Normalize */
img {
	vertical-align: bottom;
}
CSS 정리
text관련
font-family:'Loto', sans-serif;
font-size:16px(기본)
color:red,#foo.rgb(255,0,0,1),jsl...
font-weight:nomal,lighter,bold,bolder,200,300,400...
fonto-style;:italic, oblique
text-align: center,left,right,ju

Design관련
border: 1px soild(deshed,dotted,double,inset,outset,groove,none)
background-image: url('../img/bg.gif');
		background-repeat: (repeat) | no-repeat | repeat-x | repeat-y
		background-position: (left top) | center | [left, center, right] [top center bottom]
		background-position: 200px 100px | 30% 50% ...
		background-size: (자기사이즈) 100% auto | auto 100% | cover
		background-size: 200px 500px
		background-attachment: fixed <-- parallax효과
		background-image: linear-gradient([각도], #9deb7f, #256225 ...);
		[각도]: to left | to left top | 45deg
		background-image: radial-gradient(#9deb7f, #256225 ...);
		background: 컬러 url() repeat position
		








layout관련
float:left,right,none
position: relative(기준점),absolute,fixd(화면을 기준점)
flex
grid

Dimension관련
width,height-고정값
max-width, max-height-최대값
min-width, min-height-최소값
maingin, padding...
