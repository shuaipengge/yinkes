<template>
	<view>
		<view class="top-bar">
			<view class="left">
				<image src="../../static/img/003.jpg"></image>
			</view>
			<view class="center">
				<image src="../../static/images/index/火@2x.png" mode=""></image>
			</view>
			<view class="right">
				<image class="serch" src="../../static/images/index/search@2x.png" mode=""></image>
				<image class="add" src="../../static/images/index/addgroup@2x.png" mode=""></image>
			</view>
		</view>
		<view class="main">
			<view class="apply">
				<friend-item></friend-item>
				<friend-item></friend-item>
				<friend-item></friend-item>
			</view>
			<view class="friends">
			
			</view>
		</view>
	</view>
</template>

<script>
	import FriendItem from '../../components/FriendItem.vue'

	export default {
		components:{
			FriendItem
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.top-bar {
		z-index: 200;
		position: fixed;
		top: 0;
		left: 0;
		width: 686rpx;
		height: 88rpx;
		background-color: $uni-bg-color;
		box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.1);
		padding: 0 32rpx;
		display: flex;
		justify-content: space-between;
		align-items: center;

		.left {
			width: 68rpx;
			height: 68rpx;

			image {
				width: 68rpx;
				height: 68rpx;
				border-radius: 16rpx;
			}
		}

		.center {
			width: 88rpx;
			height: 42rpx;
			padding-left: 44rpx;

			image {
				width: 88rpx;
				height: 42rpx;
			}
		}

		.right {
			width: 140rpx;
			height: 52rpx;
			display: flex;
			justify-content: space-between;
			align-items: center;

			.serch {
				width: 52rpx;
				height: 52rpx;
			}

			.add {
				width: 48rpx;
				height: 48rpx;
			}
		}
	}
	.main{
		margin-top: 88rpx;
	}
</style>
