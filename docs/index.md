---
layout: home

hero:
  name: Wem Search
  text: 做一个简洁的搜索
  tagline: 搜索引擎：Bing
  image:
    src: /bing.png
    alt: VitePress
  actions:
    - theme: brand
      text: Modrinth
      link: https://modrinth.com
    - theme: alt
      text: Google
      link: https://Wemsearch.github.io/google.html
features:

---

<style>
@import url('https://fonts.googleapis.com/css?family=Cairo');
:root {
  --vp-home-hero-name-color: transparent;
  --vp-home-hero-name-background: -webkit-linear-gradient(120deg, #bd34fe 30%, #41d1ff);

  --vp-home-hero-image-background-image: linear-gradient(-45deg, #bd34fe 50%, #47caff 50%);
  --vp-home-hero-image-filter: blur(44px);
}

@media (min-width: 640px) {
  :root {
    --vp-home-hero-image-filter: blur(56px);
  }
}

@media (min-width: 960px) {
  :root {
    --vp-home-hero-image-filter: blur(68px);
  }
}


body {
	background-color: #010;
}

.htitle {
	font-family: "Cairo";
	text-align: center;
	color: #FFF;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	height: 100vh;
	letter-spacing: 1px;
	line-height:2
}

h1 {
	background-image: url(https://media.giphy.com/media/26BROrSHlmyzzHf3i/giphy.gif);
	background-size: cover;
	color: transparent;
	-moz-background-clip: text;
	-webkit-background-clip: text;
	text-transform: uppercase;
	font-size: 120px;
	margin: 10px 0;
}
/* styling my button */

.white-mode {
	text-decoration: none;
	padding: 7px 10px;
	background-color: #122;
	border-radius: 3px;
	color: #FFF;
	transition: .35s ease-in-out;
	position: absolute;
	left: 15px;
	bottom: 15px;
	font-family: "Montserrat";
}

.white-mode:hover {
	background-color: #FFF;
	color: #122;
}

/* === removing default button style ===*/
.button {
  margin: 0;
  height: auto;
  background: transparent;
  padding: 0;
  border: none;
  cursor: pointer;
}

/* button styling */
.button {
  --border-right: 6px;
  --text-stroke-color: rgba(255,255,255,0.6);
  --animation-color: #37FF8B;
  --fs-size: 2em;
  letter-spacing: 3px;
  text-decoration: none;
  font-size: var(--fs-size);
  font-family: "Arial";
  position: relative;
  text-transform: uppercase;
  color: transparent;
  -webkit-text-stroke: 1px var(--text-stroke-color);
}
/* this is the text, when you hover on button */
.hover-text {
  position: absolute;
  box-sizing: border-box;
  content: attr(data-text);
  color: var(--animation-color);
  width: 0%;
  inset: 0;
  border-right: var(--border-right) solid var(--animation-color);
  overflow: hidden;
  transition: 0.5s;
  -webkit-text-stroke: 1px var(--animation-color);
}
/* hover */
.button:hover .hover-text {
  width: 100%;
  filter: drop-shadow(0 0 23px var(--animation-color))
}
/* 这里是搜索框的css */
.input {
  margin: 0px;
  margin-top: 180px;
  width:600px;
  background: none;
  border: none;
  outline: none;
  padding: 10px 30px;
  font-size: 16px;
  border-radius: 9999px;
  box-shadow: inset 3px 8px 15px rgb(5, 5, 5);
  color: #fff;
}
.main{
	text-align: center; /*让div内部文字居中*/
	border-radius: 20px;
	width: 800px;
	height: 350px;
	margin: auto;
	position: absolute;
	top: 0;
	left: 0;
	right: 0;
	bottom: 0;
}
</style>

<div class="main">
	<form action="https://cn.bing.com/search" target="_self" method="get"  >
		<input width="500" placeholder="输入以搜索" class="input" type="text" name="q">
		<input width="500" type="submit" id="search-button" value=" ">
	</form>
</div>