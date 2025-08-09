<template>
  <div class="side-panel">
    <NuxtLink to="#">
      <Icon name="my-icon:home" size="24" />
    </NuxtLink>

    <NuxtLink to="#">
      <Icon name="my-icon:exit" size="24" />
    </NuxtLink>
  </div>
</template>
<style scoped>
.side-panel {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  background: #eee;
  padding: 42px 28px;
}

.side-panel .iconify {
  color: var(--color-black-2);
}

.side-panel a:hover .iconify {
  color: var(--color-gray);
}
</style>
