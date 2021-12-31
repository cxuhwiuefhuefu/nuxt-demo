<!--
 * @Author: Sunny
 * @Date: 2021-12-31 10:10:14
 * @LastEditors: Suuny
 * @LastEditTime: 2021-12-31 10:13:52
 * @Description:
 * @FilePath: \nuxt-demo\layouts\error.vue
-->
<template>
  <div>
    <h2 v-if="error.statusCode == 404">404页面不存在</h2>
    <h2 v-else>500服务器错误</h2>
    <ul>
      <li>
        <nuxt-link to="/"> HOME </nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: ['error']
}
</script>
