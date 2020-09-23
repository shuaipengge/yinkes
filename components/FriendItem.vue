<template>
	<view>
		<view class="friends-item">
			<view class="left">
				<image src="../static/img/001.jpg"></image>
				<text>1</text>
			</view>
			<view class="right">
				<view class="top">
					<view class="name">
						{{msg.name}}
					</view>
					<view class="time">
						{{msg.time}}
					</view>
				</view>
				<view class="down">
					<view class="msg">
						{{msg.msg}}
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				msg: {
					headimg: '../static/img/002.jpg',
					name: '高级前端开发',
					msg: '今天不用加班早点回家打游戏、追剧、看电影、吃饭、睡觉',
					time: '上午7:40'
				}
			};
		}
	}
</script>

<style lang="scss">
	.friends-item {
		padding: 0 $uni-spacing-col-base;
		width: 750rpx;
		// height: 128rpx;
		padding: 18rpx 32rpx 14rpx 32rpx;
		display: flex;
		align-items: center;

		.left {
			width: 96rpx;
			height: 96rpx;
			position: relative;

			image {
				width: 96rpx;
				height: 96rpx;
				border-radius: $uni-border-radius-base;
			}

			text {
				position: absolute;
				top: -10rpx;
				left: 76rpx;
				width: 36rpx;
				height: 36rpx;
				text-align: center;
				line-height: 36rpx;
				color: $uni-text-color-inverse;
				font-size: $uni-font-size-sm;
				background-color: $uni-color-warning;
				border-radius: $uni-border-radius-circle;
			}
		}

		.right {
			padding-left: 32rpx;
			width: 560rpx;

			.top {
				display: flex;
				justify-content: space-between;
				align-items: center;
				height: 50rpx;

				.name {
					font-size: 36rpx;
					font-weight: 400;
					color: $uni-text-color;
					line-height: 50rpx;
				}

				.time {
					font-size: $uni-font-size-sm;
					font-weight: 400;
					color: $uni-text-color-disable;
					line-height: 34px;

				}
			}

			.down {
				height: 40rpx;

				.msg {
					height: 40rpx;
					font-size: 29rpx;
					font-weight: 400;
					color: $uni-text-color-grey;
					line-height: 40rpx;
					overflow: hidden;
					text-overflow: ellipsis;
					display: -webkit-box;
					-webkit-line-clamp: 1;
					-webkit-box-orient: vertical;
					// todo 改为SCSS函数
				}
			}
		}
	}
</style>
