<template>
  <a-space>
    服务器ip选择：
    <a-select
      ref="select"
      v-model:value="value1"
      style="width: 120px"
      :options="options1"
      @focus="focus"
      @change="handleChange"
      placeholder="请根据所在区选择服务器"
    ></a-select>
  </a-space>
</template>
<script>
import { defineComponent, ref } from 'vue'
export default defineComponent({
  setup () {
    const options1 = ref([
      {
        value: 'jack',
        label: '默认服务器'
      },
      {
        value: 'jack',
        label: '从化区服务器'
      },
      {
        value: 'lucy',
        label: 'Lucy'
      },
      {
        value: 'yiminghe',
        label: 'Yiminghe'
      }
    ])
    const focus = () => {
      console.log('focus')
    }
    const handleChange = (value) => {
      console.log(`selected ${value}`)
    }
    return {
      focus,
      handleChange,
      value1: ref('默认服务器'),
      options1
    }
  }
})
</script>
