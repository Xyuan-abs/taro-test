<script setup>
import { ref } from 'vue'

defineProps({
  title: {
    type: String,
    default: '',
  },
})

let emit = defineEmits(['change'])
const msg = ref('test')

setTimeout(() => {
  emit('change', 'test change')
}, 2000)

defineExpose({
  msg,
})
</script>

<template>
  <view class="test">
    <text>{{ msg }}{{ title }}</text>
  </view>
</template>
