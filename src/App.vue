<script setup>
import { DeleteTwoTone } from '@ant-design/icons-vue';
import { ref } from 'vue'

const value = ref('');
</script>

<template>
  <section class="wrapper">
    <div class="container">
      <a-typography-title >Todo App</a-typography-title>
      <a-row>
        <a-col :span="24">
          <form class="todo-input" action="">
            <a-input v-model:value="value" placeholder="Add Something To Do" size="large" />
            <a-button type="primary" size="large">Add Todo</a-button>
          </form>
        </a-col>
      </a-row>
      <a-divider orientation="left">Todos</a-divider>
      <a-row :gutter="24">
        <a-col :span="12">
          <div class="todo-item">
            <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
            <a-divider orientation="center">
              <a-button size="large" shape="circle">
                <template #icon><delete-two-tone /></template>
              </a-button>
            </a-divider>
          </div>
        </a-col>
        <a-col :span="12">
          <div class="todo-item">
            <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
            <a-divider orientation="center">
              <a-button size="large" shape="circle">
                <template #icon><delete-two-tone /></template>
              </a-button>
            </a-divider>
          </div>
        </a-col>
        <a-col :span="12">
          <div class="todo-item">
            <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
            <a-divider orientation="center">
              <a-button size="large" shape="circle">
                <template #icon><delete-two-tone /></template>
              </a-button>
            </a-divider>
          </div>
        </a-col>
        <a-col :span="12">
          <div class="todo-item">
            <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
            <a-divider orientation="center">
              <a-button size="large" shape="circle">
                <template #icon><delete-two-tone /></template>
              </a-button>
            </a-divider>
          </div>
        </a-col>
        <a-col :span="12">
          <div class="todo-item">
            <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
            <a-divider orientation="center">
              <a-button size="large" shape="circle">
                <template #icon><delete-two-tone /></template>
              </a-button>
            </a-divider>
          </div>
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

  .todo-input {
    display: flex;
    align-items: center;
    gap: 24px;
    width: 100%;
  }

  .todo-item {
    width: 100%;
    background-color: #fff;
    border: 1px solid rgba(0, 0, 0, 0.06);
    margin-top: 12px;
    margin-bottom: 12px;

    .ant-typography {
      text-align: center;
      padding: 16px 16px 0;
    }
  }
</style>
