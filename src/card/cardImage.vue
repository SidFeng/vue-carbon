<template>
<div class="vc-card-image">
  <img :src="src" width="100%" height="100%"/>
  <slot></slot>
</div>
</template>

<script>
export default {
  props: {
    src: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="less">
.vc-card-image{
  position: relative;
  height: 40vw;
  img{
    width: 100%;
    height: 100%;
  }
  .vc-card-title{
    color: #fff;
    font-size: 1.6px;
    position: absolute;
    bottom: 4px;
    left: 16px;
  }
}
</style>
