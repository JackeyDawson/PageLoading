<template>
	<view class="content">
		<h1>CSS LOADERS</h1>
		<loader :loaderKey="index+1" v-for="(item,index) in 42" :key="index"></loader>
	</view>
</template>

<script>
	import loader from '@/components/loader/loader.vue'
	export default {
		components: {
			loader
		},
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
	.content {
		text-align: center;
	}
</style>
