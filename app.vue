<script setup>
import { useFetch } from "nuxt/app";

const { data } = await useFetch("https://api.example.com/data");
</script>

<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtPage />
  </div>
</template>
