<template>
  <div class="loading">
    <img src="../../static/images/ajax-loader.gif" alt="">
  </div>
</template>
<script>
  export default {
    name: 'load'
  }
</script>
<style lang="less">
  .loading {
    position: relative;
    top: 0;
    left: 0;
    height: 100vh;
    text-align: center;
    img {
      width: 1rem;
      margin-top: 50%;
    }
  }
</style>
