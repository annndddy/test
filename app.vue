<script setup lang="ts">
const value = ref()
const options = ref([{value: 123, label: 'abc'}])
</script>
<template>
  <div>
    <el-select v-model="value" class="m-2" placeholder="Select" size="large">
      <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value" />
    </el-select>
    <el-button>Default</el-button>
    <NuxtWelcome />
  </div>
</template>
<style>
@import 'element-plus/dist/index.css';
</style>