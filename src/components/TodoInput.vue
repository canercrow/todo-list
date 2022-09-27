<script lang="ts" setup>
  import { ref } from 'vue'

  const value = ref('')
</script>

<template>
  <form class="todo-input" action="">
    <a-input v-model:value="value" placeholder="Add Something To Do" size="large" />
    <a-button type="primary" size="large">Add Todo</a-button>
  </form>
</template>

<style lang="scss">
  .todo-input {
    display: flex;
    align-items: center;
    gap: 24px;
    width: 100%;
  }
</style>