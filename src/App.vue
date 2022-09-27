<script setup>
  import TodoInput from './components/TodoInput.vue'
  import TodoItem from './components/TodoItem.vue'
</script>

<template>
  <section class="wrapper">
    <div class="container">
      <a-typography-title >Todo App</a-typography-title>
      <a-row>
        <a-col :span="24">
          <TodoInput />
        </a-col>
      </a-row>
      <a-divider orientation="left">Todos</a-divider>
      <a-row :gutter="24">
        <a-col :span="12">
          <TodoItem />
        </a-col>
        <a-col :span="12">
          <TodoItem />
        </a-col>
        <a-col :span="12">
          <TodoItem />
        </a-col>
        <a-col :span="12">
          <TodoItem />
        </a-col>
        <a-col :span="12">
          <TodoItem />
        </a-col>
      </a-row>
    </div>
  </section>
</template>

<style lang="scss">
  .wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;
    padding: 100px 0;
  }
  .container {
    width: 100%;
    max-width: 1040px;
    padding-left: 24px;
    padding-right: 24px;
    margin: 0 auto;
  }
</style>
