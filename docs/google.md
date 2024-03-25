---
layout: home

hero:
  name: Wem Search
  text: 做一个简洁的搜索
  tagline: 搜索引擎：Google
  image:
    src: /bing.png
    alt: VitePress
  actions:
    - theme: brand
      text: Modrinth
      link: https://modrinth.com
    - theme: alt
      text: Bing
      link: https://Wemsearch.github.io
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


/* 这里是搜索框的css */
.input {
  margin: 0px;
  margin-top: 180px;
  width:600px;
  background: none;
  border: none;
  outline: none;
  padding: 16px 30px;
  font-size: 16px;
  border-radius: 9999px;
  box-shadow: inset 4px 10px 17px rgb(7, 5, 10);
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
	<form action="https://www.google.com/search" target="_self" method="get"  >
		<input width="500" placeholder="输入以搜索" class="input" type="text" name="q">
		<input width="500" type="submit" id="search-button" value=" ">
	</form>
</div>
