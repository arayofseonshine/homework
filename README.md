# homework# homework
html 코드

각각 4개의 아바타 div를 포함한 섹션 2개
<div class="avatars1">
 <div class="avatars2">

각각의 아바타 div는 이미지와 상태 정보를 포함
<div class="avatar">
이미지는 아래 태그로 나타냄
   	<img src="../images/faces/face1.jpg" art="">
	상태정보는 아래 태그로 나타냄
            	<div class="status off"></div>

각 아바타의 상태를 나타내는 클래스 
<div class="status on"></div>.
<div class="status off"></div>




css 코드 

각각의 아바타 그룹을 나타냄 
.avatars1(2){
		display: flex; // 그룹 내 아바타들 가로 배열 
		justify-content: center; // 그룹 내 아바타들 가운데 정렬
}


아바타 그룹 내 이미지를 꾸밈
.avatars1(2) img {
    border-radius: 50%; // 이미지를 원형으로
    width: 64px; // 이미지 크기
    height: 64px; // 이미지 크기
		margin: 10px; // 이미지 주변의 공간 
}

아바타를 나타냄
.avatar{
	position: relative; // 요소 내의 절대적 위치
	display: inline-block; // 요소를 인라인 블록으로 
}

아바타의 상태
.status{
	position: absolute; // 상태요소를 아바타 요소에 상대적으로 배치
	right: 3px; // 위치 
	bottom: 10px; // 위치 
	width: 17px; // 상태 요소의 크기
	height: 17px; // 상태 요소의 크기 
	border-radius: 50%; // 원형
	border: medium solid white; // 상태 요소 주변에 흰색 실선 테두리 

아바타의 상태
.status.on{
	background-color: #4CFE88;
}
.status.off {
	background-color: #DBDBDB;
}

}