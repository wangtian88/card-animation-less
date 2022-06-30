<template>
  <div class="visual-card flex flex-nowrap">
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
      transform: rotateY(360deg);
    }
  }

  @transform1: rotateY(45deg) translateZ(-800px);
  @transform2: rotateY(45deg) translateZ(-600px);
  @transform3: rotateY(45deg) translateZ(-400px);
  @transform4: rotateY(-45deg) translateZ(-400px);
  @transform5: rotateY(-45deg) translateZ(-600px);
  @transform6: rotateY(-45deg) translateZ(-800px);

  @keyframes dh1 {
    0% {
      transform: @transform1;
    }

    8.33% {
      transform: @transform1;
    }

    16.66% {
      transform: @transform2;
    }

    24.99% {
      transform: @transform2;
    }

    33.32% {
      transform: @transform3;
    }

    41.65% {
      transform: @transform3;
    }

    49.98% {
      transform: @transform4;
    }

    58.31% {
      transform: @transform4;
    }

    66.64% {
      transform: @transform5;
    }

    74.97% {
      transform: @transform5;
    }

    83.3% {
      transform: @transform6;
    }

    91.63% {
      transform: @transform6;
    }

    100% {
      transform: @transform1;
    }
  }

  @keyframes dh2 {
    0% {
      transform: @transform2;
    }

    8.33% {
      transform: @transform2;
    }

    16.66% {
      transform: @transform3;
    }

    24.99% {
      transform: @transform3;
    }

    33.32% {
      transform: @transform4;
    }

    41.65% {
      transform: @transform4;
    }

    49.98% {
      transform: @transform5;
    }

    58.31% {
      transform: @transform5;
    }

    66.64% {
      transform: @transform6;
    }

    74.97% {
      transform: @transform6;
    }

    83.3% {
      transform: @transform1;
    }

    91.63% {
      transform: @transform1;
    }

    100% {
      transform: @transform2;
    }
  }

  @keyframes dh3 {
    0% {
      transform: @transform3;
    }

    8.33% {
      transform: @transform3;
    }

    16.66% {
      transform: @transform4;
    }

    24.99% {
      transform: @transform4;
    }

    33.32% {
      transform: @transform5;
    }

    41.65% {
      transform: @transform5;
    }

    49.98% {
      transform: @transform6;
    }

    58.31% {
      transform: @transform6;
    }

    66.64% {
      transform: @transform1;
    }

    74.97% {
      transform: @transform1;
    }

    83.3% {
      transform: @transform2;
    }

    91.63% {
      transform: @transform2;
    }

    100% {
      transform: @transform3;
    }
  }

  @keyframes dh4 {
    0% {
      transform: @transform4;
    }

    8.33% {
      transform: @transform4;
    }

    16.66% {
      transform: @transform5;
    }

    24.99% {
      transform: @transform5;
    }

    33.32% {
      transform: @transform6;
    }

    41.65% {
      transform: @transform6;
    }

    49.98% {
      transform: @transform1;
    }

    58.31% {
      transform: @transform1;
    }

    66.64% {
      transform: @transform2;
    }

    74.97% {
      transform: @transform2;
    }

    83.3% {
      transform: @transform3;
    }

    91.63% {
      transform: @transform3;
    }

    100% {
      transform: @transform4;
    }
  }

  @keyframes dh5 {
    0% {
      transform: @transform5;
    }

    8.33% {
      transform: @transform5;
    }

    16.66% {
      transform: @transform6;
    }

    24.99% {
      transform: @transform6;
    }

    33.32% {
      transform: @transform1;
    }

    41.65% {
      transform: @transform1;
    }

    49.98% {
      transform: @transform2;
    }

    58.31% {
      transform: @transform2;
    }

    66.64% {
      transform: @transform3;
    }

    74.97% {
      transform: @transform3;
    }

    83.3% {
      transform: @transform4;
    }

    91.63% {
      transform: @transform4;
    }

    100% {
      transform: @transform5;
    }
  }

  @keyframes dh6 {
    0% {
      transform: @transform6;
    }

    8.33% {
      transform: @transform6;
    }

    16.66% {
      transform: @transform1;
    }

    24.99% {
      transform: @transform1;
    }

    33.32% {
      transform: @transform2;
    }

    41.65% {
      transform: @transform2;
    }

    49.98% {
      transform: @transform3;
    }

    58.31% {
      transform: @transform3;
    }

    66.64% {
      transform: @transform4;
    }

    74.97% {
      transform: @transform4;
    }

    83.3% {
      transform: @transform5;
    }

    91.63% {
      transform: @transform5;
    }

    100% {
      transform: @transform6;
    }
  }

  body {
    background-color: rgb(16, 14, 14);
  }

  .visual-card {
    position: absolute;
    top: 270px;
    bottom: 375px;
    width: 100%;
    left: 50%;
    transform: translateX(-50%);
    z-index: 100;
  }

  .contain {
    margin: 0;
    padding: 0;
    /* 设置flex布局 */
    display: flex;
    /* 在主轴上居中 */
    justify-content: center;
    /* 在测轴上居中 */
    align-items: center;
    height: 100%;
    width: 100%;
    /* 透视 */
    perspective: 900px;
  }

  .section-box {
    width: 291px;
    height: 387px;
    position: relative;
    /* 所有子元素在3D空间中呈现。 */
    transform-style: preserve-3d;

    .card-box {
      position: absolute !important;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      display: flex;
      vertical-align: middle;
      /* 图片居中 */
      text-align: center;
      /* 设置图片倒影 */
      -webkit-box-reflect: below 15px linear-gradient(transparent 10%, rgba(255, 255, 255, 0.3));
      animation-duration: 15s;
      animation-timing-function: linear;
      animation-iteration-count: infinite;
      animation-delay: 3s;

      &:nth-child(1) {
        transform: @transform1;
        animation-name: dh1;
        background-color: aqua;
      }

      &:nth-child(2) {
        transform: @transform2;
        animation-name: dh2;
        background-color: burlywood;
      }

      &:nth-child(3) {
        transform: @transform3;
        animation-name: dh3;
        background-color: thistle;
      }

      &:nth-child(4) {
        transform: @transform4;
        animation-name: dh4;
        background-color: coral;
      }

      &:nth-child(5) {
        transform: @transform5;
        animation-name: dh5;
        background-color: crimson;
      }

      &:nth-child(6) {
        transform: @transform6;
        animation-name: dh6;
        background-color: deeppink;
      }
    }
  }

  .trans(@trans) {
    transform: @trans;
  }

  .card-animation(@n, @i:1) when (@i <= @n) {
    &:nth-child(@{i}) {
      transform: ` @{transform @{i}}`;
    }

    .card-animation(@n,(@i + 1));
  }
</style>
