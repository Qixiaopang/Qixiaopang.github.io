
<template>
  <div id="app">
  	<div class="banner">
  			<nav class="nav">
  					<div>
  						<a href="javascript:;">主页</a>
  						<a href="javascript:;">简介</a>
  						<a href="javascript:;">工作经历</a>
  						<a href="javascript:;">案例展示</a>
  						<a href="javascript:;">联系方式</a>
  					</div>
  			</nav>
  			<div class="ban_center">
  					<i></i>
  					<p class="my">世上只有想不通的人，没有走不通的路。</p>
  					<hr />
  					<p class="name">齐弦</p>
  					<p class="name">20岁</p>
  					<p class="name">Web前端工程师</p>
  					<p class="name">18210837762</p>
  			</div>
  			
  	</div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
*{margin: 0;padding: 0;}
a{list-style: none;text-decoration: none;}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.banner{
	width: 100%;
	height: 493px;
	background: url(assets/img.png) center no-repeat;
	/*background-size: 100%;*/
	padding-top: 160px;
}
.nav{
	width: 100%;
	height: 60px;
	background:rgb(35,42,71);
	position: fixed;
	top: 0;
	left: 0;
}
.nav>div{
	width: 33%;
	height: 60px;
	margin: 0 auto;
}
.nav>div>a{
	display: block;
	float: left;
	padding: 0 10px;
	height: 60px;
	line-height: 60px;
	text-align: center;
	color: #fff;
}
.nav>div>a:hover{
	background:rgb(80,84,103);
	color: #fff;
}
.ban_center{
	width: 60%;
	height: 493px;
	/*background: #fff;*/
	margin: 0 auto;
}
.ban_center>i{
	display: block;
	width: 112px;
	height: 112px;
	background: url(assets/56_192926_9.jpg) no-repeat center;
	background-size: 112px 112px;
	overflow: hidden;
	border-radius: 50%;
	margin: 0 auto 20px;
}
.my{
	color: #fff;
  font-size: 24px;
  text-align: center;
  margin-bottom: 10px;
}
.ban_center>hr{
	width: 70%;
    height: 1px;
    background: #999999;
    border: 0;
    margin: 0 auto 5% auto;
    opacity: 1;
    animation: 1s to_width ease-in 0s 1;
}
@keyframes to_width{
	0% {
	    width: 0;
	    opacity: 0;
	}
	50% {
	    width: 40%;
	    opacity: 0.5;
	}
	100% {
	    width: 70%;
	    opacity: 1;
	}
}
.name{
	color: #fff;
  font-size: 20px;
  text-align: center;
  margin: 10px 0;
}
</style>
