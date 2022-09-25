<template>
	<view class="page">
		<view class="header">
				<!-- <input class="uni-input" focus placeholder="自动获得焦点" /> -->
				<!-- <button class="mini-btn" type="primary" size="mini">按钮</button> -->
				<view slot="default" class="search_box">
					<text class="iconfont">&#xe6e1</text>
					<input style="width: 280px;" :value="searchName" class="prompt" placeholder="请输入查询关键字" @input="theBlur"></input>
				</view>
		</view>
	 	<view class="content">
			123
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value: ""
			}
		},
		methods: {
			theBlur(){}
		}
	}
</script>

<style lang="scss">
	@import url("@/static/nav/iconfont.css");
	.page{
		display: -webkit-flex; /* Safari */
		display: flex;
		flex-direction: column;
		height: 100%;
	}
	.header{
		display: flex;
		justify-content: center;
		/* background-color: red;s */
	}
	.content{
		background-color: #000;
	}
	.btn-search{
		
	}
	.search_box {
			width: 400upx;
			height: 64upx;
			background-color: #f5f5f5;
			border-radius: 32upx;
			display: flex;
			align-items: center;
			padding: 0upx 40upx;
			.prompt {
				font-size: 28upx;
				color: #cccccc;
			}
		}
		
		.iconfont  {
			background-position: center center;
			background-repeat: no-repeat;
			background-size: cover;
			width: 32upx;
			height: 28upx;
			margin-right: 20rpx;
		}
		
		.icon_close {
			background-position: center center;
			background-repeat: no-repeat;
			background-size: cover;
			width: 32upx;
			height: 28upx;
			margin-right: 10rpx;
		}
</style>
