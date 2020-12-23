<template>
	<view class="content">
		<div class="container">
		    <button class="btn btn1">Hover Me</button>
		    <button class="btn btn2">Hover Me</button>
		    <button class="btn btn3">Hover Me</button>
		    <button class="btn btn4">Hover Me</button>
		</div>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="less">
	page {
		margin: 0;
		padding: 0;
		background: #e0e5ec;
	}
	.container {
		perspective:320px;
	}
	.btn {
		display:block;
		margin:40px auto;
		width:240px;
		height:100rpx;
		border:none;
		background-color:#00a8ff;
		color:#fff;
		font-size:18px;
		border-radius:6px;
		outline:none;
		cursor:pointer;
		transition:.3s linear;
	}
	.btn1:hover {
		transform:rotateX(15deg);
		box-shadow:0 15px 15px rgba(89,195,255,0.58);
	}
	.btn2:hover {
		transform:rotateX(-15deg);
		box-shadow:0 -15px 15px rgba(89,195,255,0.58);
	}
	.btn3:hover {
		transform:rotateY(15deg);
		box-shadow:-15px 0 15px rgba(89,195,255,0.58);
	}
	.btn4:hover {
		transform:rotateY(-15deg);
		box-shadow:15px 0 15px rgba(89,195,255,0.58);  
	}


</style>
