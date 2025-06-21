<script setup lang="ts">
import { NConfigProvider, NDynamicTags, type GlobalThemeOverrides } from 'naive-ui'

const override: GlobalThemeOverrides = {
  DynamicTags: {
    peers: {
      Tag: {
        color: 'red'
      }
    }
  }
}
</script>

<template>
  <n-config-provider :theme-override="override">
    <n-dynamic-tags :value="['123', '456']"></n-dynamic-tags>
  </n-config-provider>
</template>
