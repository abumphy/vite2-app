<template>
  <div>
    <h4>{{ msg }}</h4>
    <van-button type="primary" @click="inc">{{count}}</van-button>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const msg = 'Hello!'

const count = ref(0)

function inc() {
  count.value++
}
</script>
<style lang='scss' scoped>
</style>