<script setup lang="ts">
import { useI18n } from 'vue-i18n';
import SignIcon from '@/components/SignIcon.vue';

const { locale } = useI18n();

function changeLocale(code: string) {
  locale.value = code;
  localStorage.setItem('pdf-signature-i18n', code);
}
</script>

<template>
  
</template>

<style lang="postcss" scoped>
.sign_header {
  @apply fixed w-full flex justify-between items-center bg-black p-2 md:p-4;
}
</style>
