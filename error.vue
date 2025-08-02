<script setup lang="ts">
import type { NuxtError } from "#app";

const { error } = defineProps<{
  error: NuxtError;
}>();

const goHome = () => {
  navigateTo("/");
};
</script>

<template>
  <div class="error-page">
    <div class="error-page__status-code">{{ error.statusCode }}</div>
    <div v-if="error.statusCode === 404" class="error-page__message">
      Страница не найдена, вернитесь на главную страницу
    </div>
    <div v-else class="error-page__message">{{ error.statusMessage }}</div>
    <UiButton class="error-page__button" @click="goHome">На главную</UiButton>
  </div>
</template>

<style scoped>
.error-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.error-page__status-code {
  font-weight: 500;
  font-size: 120px;
  line-height: 100%;
  letter-spacing: 0%;
  color: var(--color-black);
}

.error-page__message {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0%;
  text-align: center;
  color: var(--color-black);
}
.error-page__button {
  width: 300px;
  margin-top: 24px;
}
</style>
