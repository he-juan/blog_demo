<template>
  <div>
      <div id="content"> 个人首页</div>
      <h1>{{blog}}</h1>
      <div  v-for="item in cityList" class='check'>
        　<div>城市名称：{{item.title}}</div>
        　<div >城市ID：{{item.id}}</div>
      </div>
  </div>
</template>

<script>
    export default {
        name: "PersonalHomepage",
        data() {
          return {
            blog: '我的博客',
            cityList:[
              { title:'北京', id:'001' },
              { title:'上海', id:'002' }
            ]
          }

        }
    }
</script>

<style scoped>
  #content {
    width: 90%;
    min-width: 800px;
    margin: 10px auto;
    font-family: "微软雅黑";
  }

  h1 {
    margin: 10px auto;
    width: 90%;
    min-width: 800px;
  }

  .check{
    margin: 10px auto;
    width: 90%;
    min-width: 800px;
  }
</style>
