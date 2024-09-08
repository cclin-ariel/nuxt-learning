<script setup>
import { useFetch } from "nuxt/app";

const { data } = await useFetch("https://api.example.com/data");
</script>

<template>
  <h1>Hello world!</h1>
</template>

<style scoped></style>
