<template>
  <div id="app">
   <header class="header" >
		 <div class="titlecontianer">
				<span class="mui-icon mui-icon-bars"></span>
			               <!-- 单击标题跳转到首页 -->
				<span class="title" @click="index()">国际仿生学术平台</span>
				<span class="mui-icon mui-icon-contact"></span>
			</div>
		 
		</header>
    <router-view></router-view>

  </div>
</template>

<script>
export default {
  name: 'app',
	methods:{
		index:function(){
			this.$router.push('/');
		}
	}
}
</script>

<style lang="less">
  .header {
		z-index: 99;
		background-color:skyblue;
		text-align:center;
		height:60px;
		line-height:60px;

		.titlecontianer{
			margin-right: 10px;
			margin-left: 10px;
	
		}

		.title{
		 font-family: "Arial","Microsoft YaHei","黑体","宋体",sans-serif;
		 font-size:18px;
		 font-weight: bold;
		 margin-right: 50px;
		 margin-left: 50px;
		}
		
	}
 
</style>
