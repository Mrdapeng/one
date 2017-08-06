<template>
  <div class="menu">
    <ul>
      <li>
        <router-link class="link-to" to="/read">阅读</router-link>
      </li>
      <li>
        <router-link class="link-to" to="/picture">图文</router-link>
      </li>
      <li>
        <router-link class="link-to" to="/music">音乐</router-link>
      </li>
      <li>
        <router-link class="link-to" to="/movie">影视</router-link>
      </li>
      <li>
        <router-link class="link-to" to="/about">关于</router-link>
      </li>
      <
    </ul>
  </div>
</template>
<script>
  export default {
    data() {
      return {}
    },
    methods: {}
  }
</script>
<style lang="less">
  .menu {
    width: 2.3rem;
    height: 100vh;
    position: absolute;
    top: 0;
    background: #fff;
    color: #000;
    left: -3rem;
    box-shadow: 4px -2px 16px 0px #adabab;
    z-index: 99;
    padding-top: 0.5rem;
    li {
      width: 2.4rem;
      .link-to {
        display: inline-block;
        padding: .1rem .3rem;
        width: 100%;
        font-size: .4rem;
        line-height: .6rem;
        text-decoration: none;
        color: #333;
      }
    }
  }

</style>
