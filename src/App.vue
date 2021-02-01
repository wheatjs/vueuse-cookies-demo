<template>
  Test Cookie: {{ cookies.get('test') }}
</template>

<script lang="ts" setup>
import { useCookies } from '@vueuse/integrations' 

const cookies = useCookies()
cookies.set('test', 'This is a test cookie')
</script>
