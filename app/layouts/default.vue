<script lang="ts" setup>
  const prismic = usePrismic()

  const { data: settings } = await useAsyncData(() => prismic.client.getSingle('settings'))
  
  useSeoMeta
</script>

<template>
  <div>
    {{ settings }}
    <slot />
  </div>
</template>