<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<popupBar size="middle" position="right"  bgColor="#10baaa">
			<view slot="main" class="refrash_wrap" @click="handleRefrash">
				<image class="icon" src="../../static/refrash.png"></image>
				<view class="text">重置</view>
			</view>
		</popupBar>
		
	</view>
</template>

<script>
	import popupBar from '@/components/popup-bar/popup-bar.vue'
	export default {
		components:{
			popupBar
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			handleRefrash() {
				this.title = 'world'
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.icon{
		width: 40rpx;
		height: 40rpx;
	}
	.refrash_wrap{
		display: flex;
		align-items: center;
	}
	.text{
		width: 60rpx;
		margin-left:10rpx;
	}
</style>
