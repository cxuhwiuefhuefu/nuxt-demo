<!--
 * @Author: Sunny
 * @Date: 2021-12-30 18:05:11
 * @LastEditors: Suuny
 * @LastEditTime: 2021-12-30 18:13:27
 * @Description:
 * @FilePath: \nuxt-demo\pages\news\_id.vue
-->
<template>
  <div>
    <h1>New-Content [{{ $route.params.id }}]</h1>
    <ul>
      <li>
        <a href="/">Home</a>
      </li>
    </ul>
  </div>
</template>

export default {
  validate({params}) {
    return /^\d+$/.test(params.id)/
  }
}
