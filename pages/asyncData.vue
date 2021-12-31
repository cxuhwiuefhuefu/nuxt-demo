<!--
 * @Author: Sunny
 * @Date: 2021-12-31 10:50:54
 * @LastEditors: Suuny
 * @LastEditTime: 2021-12-31 10:50:54
 * @Description: 
 * @FilePath: \nuxt-demo\pages\asyncData.vue
-->
<template>
  <div>
    <h1>姓名：{{info.name}}</h1>
    <h1>年龄：{{info.age}}</h1>
    <h1>兴趣：{{info.interest}}</h1>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  data () {
    return 'hello world'
  },
  async asyncData() {
    // return axios.get('https://api.myjson.com/bins/8gdmr')
    //   .then((res)=>{
    //       console.log(res)
    //       return {info:res.data}
    //   })

   let {data} = await axios.get('https://api.myjson.com/bins/8gdmr')
   return {info: data}  
  }
}
</script>