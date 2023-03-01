<template>
  <nut-input v-model="id" placeholder="请输入身份证" type="idcard" />
  <nut-button type='primary' @click="getId">获取身份证</nut-button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const id = ref<string>('')

const getId = () => {
  console.log('id', id.value);
}
</script>

<style lang="scss">
.index {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
