<script lang="ts" setup>
import { WOW } from 'wowjs'
import 'animate.css'
const { title, description } = useAppConfig()
useHead({
  title,
  meta: [{
    name: 'description',
    content: description
  }]
})
const wow = new WOW({
  boxClass: 'wow',
  animateClass: 'animated',
  offset: 100,
  mobile: true,
  live: true
})
wow.init()
</script>
<template>
  <NuxtPage />
</template>
