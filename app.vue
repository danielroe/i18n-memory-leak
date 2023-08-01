<template>
  <span>{{ timeLabel }}</span>
</template>

<script lang="ts" setup>
const { $i18n } = useNuxtApp()

await new Promise(resolve => setTimeout(resolve, 10))

const timeLabel = computed(() => $i18n.t('general'))
</script>

