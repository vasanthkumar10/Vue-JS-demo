<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ["mode"],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  border: 1px solid #3a0061;
  background-color: #3a0061;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  border-color: #270041;
  background-color: #270041;
  text-decoration: underline;
  text-underline-offset: 1px;
}

.flat {
  background-color: transparent;
  color: #3a0061;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: transparent;
}
</style>
