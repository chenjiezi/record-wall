<script setup>
import { ref } from "vue";
const list = ref([
  "测试数据测试数据测试数据测试数据测试数据测试数据测试数据",
  "测试数据测试数据测试数据测试数据测试数据测试数据测试数据",
  "测试数据测试数据测试数据测试数据测试数据测试数据测试数据",
  "测试数据测试数据测试数据测试数据测试数据测试数据测试数据",
  "测试数据测试数据测试数据测试数据测试数据测试数据测试数据",
]);
</script>

<template>
  <div class="w-100% min-h-screen flex flex-wrap bg-gray-500 p-10px">
    <div
      class="w-250px h-60px bg-blue-400 m-r12px mb-12px border-rd flex items-center p-10px"
      v-for="item in list"
      :key="item"
    >
      <div class="w-45px h-45px mr-12px flex-shrink-0">
        <img
          src="https://dummyimage.com/50x50/000/fff"
          alt=""
          class="w-full h-full border-rd-50"
        />
      </div>
      <div class="inline-block text-light-50">{{ item }}</div>
    </div>
  </div>
</template>
