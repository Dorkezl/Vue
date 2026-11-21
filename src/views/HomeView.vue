<script setup>
import { ref } from 'vue'

const world = '世界'
const flag = false
const list1 = ref([
  { id: 1, name: '张三' },
  { id: 2, name: '李四' },
  { id: 3, name: '王五' },
])
</script>

<template>
  <main>
    <h1>首页</h1>
    <p>你好，{{ world }}</p>
  </main>
  <div v-if="flag">Hello</div>
  <div v-else>Vue</div>
  <div v-show="flag">你好,Vue</div>
  <ul>
    <li v-for="value in list1" :key="value.id">
      {{ value.name }}
    </li>
  </ul>
</template>
