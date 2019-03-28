# WoouTGD
트위치 우유쪼아 [트게더 페이지](https://tgd.kr/woou012) 커스텀 CSS

## 사용법
### 1. 색상 조정
색상은 크게 아래 네 가지로 나뉘어져 있으며, :root의 색상을 조정해주면 자동으로 바뀜.
<pre><code>
:root {
	--primary-color: #ff6b6b;
	--secondary-color: #ffbebe;
	--component-color: transparent;
	--component-secondary-color: #ffeeee;
}
</code></pre>

### 2. 배경 이미지 리소스 변경
배경 이미지는 [다콩 트게더](https://tgd.kr/dakong_)를 참조했음. 아래 속성의 세 이미지 링크를 변경할 수 있음.
<pre><code>
body {
	background: url('../res/img/1.png'), url('../res/img/2.png'), url('../res/img/3.png'), #FFFFFF;
	animation: background 20s linear infinite;
}
</code></pre>

애니메이션 정의는 다음과 같음. 
<pre><code>
/*animations*/
@keyframes background {

    0% {
        background-position: 0px 0px, 0px 0px, 0px 0px;
    }

    100% {
        background-position: 500px 1000px, 400px 400px, 300px 300px;
    }

}
/*animations end*/
</code></pre>

리소스 관리는 이미지 호스팅을 추천하나, 본 repository에 업로드하여 github page의 호스팅을 받는것을 추천함.
