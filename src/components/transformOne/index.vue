<template>
	<div class="contain">
		<section class="section-box">
			<div class="card-box">
				<img src="../../assets/images/1.png" />
			</div>
			<div class="card-box">
				<img src="../../assets/images/2.png" />
			</div>
			<div class="card-box">
				<img src="../../assets/images/3.png" />
			</div>
			<div class="card-box">
				<img src="../../assets/images/4.png" />
			</div>
			<div class="card-box">
				<img src="../../assets/images/5.png" />
			</div>
			<div class="card-box">
				<img src="../../assets/images/6.png" />
			</div>
		</section>
	</div>
</template>

<script lang="ts" setup>
</script>

<style lang="less">
  /* 整体旋转动画 */
    @keyframes dh {
      from {
        /* 起始角度 */
        transform: rotateY(0deg);
      }
 
      to {
        /* 最终角度 */
        transform: rotateY(360deg)
      }
    }

	.contain {
		/* 设置flex布局 */
		display: flex;
		/* 在主轴上居中 */
		justify-content: center;
		/* 在测轴上居中 */
		align-items: center;
		height: 100vh;
		background-color: #000000;
		/* 透视 */
		perspective: 900px;

		.section-box {
			width: 300px;
      height: 200px;
      position: relative;
      /* 所有子元素在3D空间中呈现。 */
      transform-style: preserve-3d;
      /* 设置动画属性 */
      animation: dh 20s linear infinite;

			.card-box {
				position: absolute;
				left: 0;
				top: 0;
				width: 100%;
				height: 100%;
				/* 图片居中 */
				text-align: center;
				/* 设置图片倒影 */
				-webkit-box-reflect: below 15px linear-gradient(transparent 10%, rgba(255, 255, 255, 0.3));

				/* 设置每一张图片的特有样式 */
				&:nth-child(1) {
					background-color: #C14C39;
					/* 在Z轴上移动300px */
					transform: translateZ(300px);
				}
		
				&:nth-child(2) {
					background-color: #6E9C72;
					/* 沿Y轴旋转0度，并在Z轴上移动300px */
					transform: rotateY(60deg) translateZ(300px);
				}
		
				&:nth-child(3) {
					background-color: #5E5F7A;
					transform: rotateY(120deg) translateZ(300px);
				}
		
				&:nth-child(4) {
					background-color: #F5EB98;
					transform: rotateY(180deg) translateZ(300px);
				}
		
				&:nth-child(5) {
					background-color: #50A3BC;
					transform: rotateY(240deg) translateZ(300px);
				}
		
				&:nth-child(6) {
					background-color: #F9A99A;
					transform: rotateY(300deg) translateZ(300px);
				}
			}
		}
	}
</style>
