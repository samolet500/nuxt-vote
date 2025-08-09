<template>
  <div class="page">
    <LayoutSidePanel />
    <LayoutContent>
      <slot></slot>
    </LayoutContent>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  height: 100vh;
  width: 100%;
}
</style>
