<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****3311 获得了三升四数学行程问题画图法 SOP"
  },
  {
    "text": "用户 189****6622 完成了五年级看图写话修辞手法引申"
  },
  {
    "text": "用户 131****9900 生成了解决作业拖延 21 天星空打卡表"
  },
  {
    "text": "用户 156****4455 完成了小学英语自然拼读口诀卡片"
  },
  {
    "text": "用户 173****8811 取得了家长辅导不发火高情商沟通话术"
  }
]);
</script>
