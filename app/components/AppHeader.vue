<script lang="ts" setup>
import type { Content } from "@prismicio/client"

defineProps<{
	settings?: Content.SettingsDocument
}>()
</script>

<template>
	<header>Header Content</header>
</template>
