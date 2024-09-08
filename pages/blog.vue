<script setup>
import { useAsyncData } from "#app";

const { data: post } = await useAsyncData("blogPost", async () => {
  // 這裡可以是實際的 API 調用
  // 例如: return await $fetch('https://api.example.com/blog-post')

  // 現在我們只是返回模擬數據
  return {
    title: "我的第一篇博客",
    content: "這是一個示例博客內容。",
  };
});
</script>

<template>
  <div v-if="post">
    <h1>{{ post.title }}</h1>
    <p>{{ post.content }}</p>
  </div>
  <p v-else>正在加載博客內容...</p>
</template>
