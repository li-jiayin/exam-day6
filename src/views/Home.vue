<template>
  <div class="home" >
    <div id = "top">
       <h4>多加网</h4>
     <div id = "search">
        <el-input placeholder="热门搜索" id = "item"></el-input>
     </div>

     
     <ul id = "nav">
       <li v-for = "(item,index) in list" :key = "index">
         <div></div>
         <p>{{item}}</p>
       </li>
     </ul>

     <ul id = "nav">
       <li v-for = "(item,index) in list" :key = "index">
         <div></div>
         <p>{{item}}</p>
       </li>
     </ul>
    </div>
    

      <!-- 轮播 -->
      <div class="block">
        <span class="demonstration">默认 Hover 指示器触发</span>
        <el-carousel height="150px">
          <el-carousel-item v-for="item in 4" :key="item">
            <h3 class="small">{{ item }}</h3>
          </el-carousel-item>
        </el-carousel>
      </div>

  </div>
</template>

<script>
 
export default {
  data(){
    return {
      list:['成单奖励','成单奖励','成单奖励','成单奖励']
    }
  }
}
</script>
