<!--
 * @Author: Sunny
 * @Date: 2021-12-30 16:53:49
 * @LastEditors: Suuny
 * @LastEditTime: 2021-12-31 11:15:46
 * @Description:
 * @FilePath: \nuxt-demo\pages\index.vue
-->
<template>
  <div>
    <img src="~static/test.jpeg" />
    <ul>
      <!-- <li><a href="/">Home</a></li>
      <li><a href="/about">ABOUT</a></li>
      <li><a href="/news">NEWS</a></li> -->
      <li>
        <nuxt-link :to="{ name: 'index' }"> HOME </nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{ name: 'about' }"> ABOUT </nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{ name: 'news', params: { newsId: 3306 } }">
          NEWS
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
