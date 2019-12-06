<template>
  <div class="home">
    <van-swipe :autoplay="3000" indicator-color="white">
      <van-swipe-item class="item">1</van-swipe-item>
      <van-swipe-item class="item">2</van-swipe-item>
      <van-swipe-item class="item">3</van-swipe-item>
      <van-swipe-item class="item">4</van-swipe-item>
    </van-swipe>
    <div class="box">
        <div v-for="(item,index) in list" :key="index">{{item}}</div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'home',
 data () {
   return {
     list:['成单奖励','成单奖励','成单奖励','成单奖励','成单奖励','成单奖励','成单奖励','成单奖励']
   }
 }
}
</script>
<style lang="scss" scoped>
.home{
  width: 100%;
  height: 200px;
 
}
.van-swipe {
    position: relative;
    overflow: hidden;
    -webkit-user-select: none;
    user-select: none;
    width: 100%;
    height: 200px;
}
.item{
  width: 100%;
  height: 200px;
  background: skyblue;
  text-align: center;
  line-height: 200px;
}
.box{
  width: 100%;
  height: 200px;
  display: flex;
  flex-wrap: wrap;
  div{
    width: 25%;
    line-height: 100px;;
    text-align: center;
  }
}
</style>