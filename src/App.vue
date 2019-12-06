<template>
  <div id="app">
    <router-link to="/home">首页</router-link>
     <router-link to="/About">我的</router-link>
    <router-view/>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
html,body,#app{
  width: 100%;
  height: 100%;
}

</style>
