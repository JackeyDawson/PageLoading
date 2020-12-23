<template>
	<view class="content">
		<view  class="bind_item" v-for="(item,index) in loadList" :key="index">
			<button size="mini" type="primary" @click="bindTab(item)">{{item}}</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				loadList:['preloader','ring','wrapper','Buttons','loader']
			}
		},
		onLoad() {

		},
		methods: {
			bindTab(item){
				uni.navigateTo({
					url:`/pages/index/${item}`
				})
			}
		}
	}
</script>

<style lang="less">
	.bind_item{
		text-align: center;
	}
</style>
