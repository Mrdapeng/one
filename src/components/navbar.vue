<template>
  <div class="header">
    <ul>
      <i class="btn_more"></i>
      <i class="search"></i>
      <li><p>一个</p></li>
      <span>{{ht}}</span>
    </ul>
  </div>
</template>
<script>
  import axios from 'axios'

  export default {
    data() {
      return {
        ht:''
      }
    },
    methods: {

      getdata() {
        axios.get("/readDetail").then(res=>{
          console.log(res)
          this.ht= res.body
        })
      }
    },
    mounted(){
      this.getdata()
    }

  }
</script>
<style scoped>
  .header {
    width: 6.4rem;
    height: 1rem;
    background: #ccc;
    position: fixed;
    top: 0;
    overflow: hidden;
  }

  .header::after {
    content: '';
    width: 0;
    height: 0;
    display: block;
    clear: both;
  }

  .header p {
    text-align: center;
    font-size: 0.5rem;
  }

  .header .btn_more {
    float: left;
    background: url('../../static/images/menu.png') no-repeat;
    background-size: 60% 60%;
    display: inline-block;
    line-height: 1rem;
    width: 1rem;
    height: 1rem;
    margin-top: 0.2rem;
  }

  .header .search {
    float: right;
    background: url('../../static/images/search.png') no-repeat;
    background-size: 60% 60%;
    display: inline-block;
    width: 1rem;
    height: 1rem;
    margin-top: 0.2rem;
  }

  .header span {
    font-size: 0.5rem;
  }

</style>
