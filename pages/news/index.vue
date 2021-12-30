<!--
 * @Author: Sunny
 * @Date: 2021-12-30 17:35:01
 * @LastEditors: Suuny
 * @LastEditTime: 2021-12-30 18:27:30
 * @Description:
 * @FilePath: \nuxt-demo\pages\news\index.vue
-->
<template>
  <div>
    <h2>News Index page</h2>
    <p>NewId: {{ $route.params.newsId }}</p>
    <ul>
      <li><a href="/">Home</a></li>
      <!-- <li><a href="/news/123">News-1</a></li>
      <li><a href="/news/456">News-2</a></li> -->
      <li>
        <nuxt-link :to="{ name: 'news-id', params: { id: 123 } }">
          News-1
        </nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{ name: 'news-id', params: { id: 456 } }">
          News-2
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>
