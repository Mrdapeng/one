<template>
  <div class="music_item">
    <h4>-音乐-</h4>
    <h2 class="music_title"></h2>
    <h3 class="sub_title"></h3>
    <img src="" alt="">
    <h5 class="music_author"></h5>
    <p class="music_article"></p>
    <span class="date"></span>
  </div>
</template>
<script>

</script>
<style lang="less">
  .music_item {
    font-size: 0.3rem;
    width: 5.8rem;
    padding: .4rem .3rem;
    background: #fff;
    margin-bottom: 1rem;
    .h4 {
      text-align: center;
    }
    .muscic_title {
      text-align: left;
    }
    .subtitle {
      text-align: left;
    }
    img{
      text-align: center;
      width: 2rem;
      height: 2rem;
      border-radius: 50% 50%;
      animation: roll linear 10s infinite;
      @keyframes roll {
        0% {transform:rotate(0deg);}
        10% {transform:rotate(36deg);}
        20% {transform:rotate(72deg);}
        30% {transform:rotate(108deg);}
        40% {transform:rotate(144deg);}
        50% {transform:rotate(180deg);}
        60% {transform:rotate(216deg);}
        70% {transform:rotate(252deg);}
        80% {transform:rotate(288deg);}
        90% {transform:rotate(324deg);}
        100% {transform:rotate(360deg);}
      }
    }
    h5{
      text-align: left;
      font-weight: 200;
    }
    .music_article{
      text-indent: 0.3rem;
      font-weight: 300;
    }
    .date{
      text-align: left;
    }
  }
</style>
