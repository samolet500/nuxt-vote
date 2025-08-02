<template>
  <button class="ui-button">
    <slot />
  </button>
</template>

<style scoped>
.ui-button {
  padding: 11px;
  border-radius: 20px;
  background: var(--color-black-2);
  border: 1px solid var(--color-black-2);
  color: var(--color-white);
  font-family: Roboto;
  font-weight: 500;
  font-style: Medium;
  font-size: 16px;
  line-height: 100%;
  text-align: center;
  cursor: pointer;
  transition: 0.2s;
}

.ui-button:hover {
  color: var(--color-black-2);
  background: var(--color-white);
}
</style>
