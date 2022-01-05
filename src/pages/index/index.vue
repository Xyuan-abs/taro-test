<script setup>
import Panel from '@/components/Panel.vue'

import { ref } from 'vue'

const msg = ref('Hello world111222')
</script>

<template>
  <panel>
    <view class="index">
      <text>{{ msg }}</text>
    </view>
  </panel>
</template>

<style lang="scss">
.index {
  background-color: red;
  width: 100px;
  text {
    color: #fff;
  }
}
</style>
