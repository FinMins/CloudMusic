<template>
	<div id="header-header">
        <div  style="width: 1320px; margin: 0 auto ">
 	<div class="header-header-container " >
		<img src="../../images/header-header.png" style="height: 70px;" alt="网易云"> 
		<a class="headr-a" href="fondMusic">发现音乐 </a>
		<a class="headr-a" href="myMusic  ">我的音乐</a>
		<a class="headr-a" href="freinds  ">朋友 	</a>
		<a class="headr-a" href="shopping ">商城 	 	</a>
		<a class="headr-a" href="musician ">音乐人    	 </a>
		<a class="headr-a" href="download ">下载客户端	</a>
	<div id="search-container">
		<form  action=" " method="GET">
		<a><img style="width:20px; height:20px" src="../../images/search-black.png" alt="搜索" > </a>
		<input id="search" type="text" name="search" :placeholder="searchDefault"  >
		</form>
	</div>
		<input id="login" type="button" onclick="a()" value="创作者中心" >
		<a id="last-a" href=" ">登录</a>
		  </div>
	</div>
</div>





</template>
<script>
export default {
    name:"Header",
    data(){
        return{
		'searchDefault':'音乐/视频/电台',
		"fondMusic" :'#',
		'myMusic  '	:'#	',
		'freinds  '	:'#	',
		"shopping "	:'#	',
		'musician '	:'#	',
		'download '	:'# '
        }
	},
	methods: {
		
	},
}
</script>



<style scoped>
/* 这里设置的body没用,作用域没那么高 */
body{
	padding: 0px;
	margin: 0px;
}

/* 大框架背景 */
#header-header{
	width: 100%;
	height:70px;
	background-color:rgb(36,36,36);
	color:white;

}
/* 中间框架 */
.header-header-container{
	display: flex;
	margin: 0;
	padding: 0;
  	 text-align: center;
  	 	height:70px;
  	 justify-content: space-between;
	   line-height: 70px;
}
/* 中间汉字链接 */
.headr-a{
	padding: 0 20px;
	 text-decoration: none;
	color:rgb(189, 189, 189);
	height:70px;

}

/* 中间汉字链接鼠标悬浮样式 */
.header-header-container a:hover{
	background-color: rgb(0,0,0);
	color: white;
}
/* 中间矿建字体 */
.header-header-container p{
	font-size:0.9em;
	height: 20px;
	margin: 35px 0 ;
}

/* 创作者中心 */
.header-header-container input{
	border-radius: 5em;
	height: 30px;
	margin:20px 0;
	padding: 0;
	border: 0;
	color: rgb(169,169,169);
	outline:none ;
}
/* 搜索的容器 */
#search-container{
	position: relative;
    width: 160px;
	height: 30px;;
	margin: 20px 0 20px 100px;
	background-color: white;
	border-radius: 15px;;
}

/* 搜索的链接 */
#search-container a{
border-top-left-radius:50%;
border-bottom-left-radius: 50%;
position: relative;
bottom:24px;
right:15px;
}

#search-container a:hover{
	background-color: white;
}
/* 搜索框 */
#search{
	position:relative;
	max-width: 100px;
	border-radius:20px;
	height: 30px;
	bottom:30px;
	right:5px;
	margin: 30px 0;
	color: rgb(164,164,164);
	background-color: white;
	border-color: rgb(36,36,36);
	/*outline:none ;
*/
}
/* 登录链接 */
#login{
	width: 100px;
	height: 32px;
	background-color: rgb(36,36,36);
	border:1px solid rgb(79,79,79) ;
	margin: 20px 0;
	line-height: 32px;
}

#login:hover{
border:1px solid white;
}

/* 登录超链接 */
#last-a{
	font-size: 0.7em;
	line-height: 70px;
	color: rgb(120, 120, 120);
	text-decoration: none;
}
#last-a:hover{
	background-color: rgb(36,36,36);
	text-decoration:underline;
}
</style>