<script setup>
import {useData, withBase} from "vitepress";
const {site, theme} = useData()
</script>

<template>
<div class="header-title">
  <a class="flex items-center" :href="withBase('/')">
    <img v-if="theme.logo" :src="withBase(theme.logo)" alt="logo" class="mr-2">
    <h1 v-if="site.title" class="text-[var(--vp-c-text-1)]">{{ site.title}}</h1>
  </a>
</div>
</template>

<style scoped>

</style>