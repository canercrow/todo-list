<script lang="ts" setup>
  import { DeleteTwoTone } from '@ant-design/icons-vue'
</script>

<template>
  <div class="todo-item">
    <a-typography-paragraph>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis eaque in animi maiores voluptas similique beatae porro assumenda natus neque quibusdam tenetur, placeat accusamus ratione! Repudiandae sit est quasi expedita!</a-typography-paragraph>
    <a-divider orientation="center">
      <a-button size="large" shape="circle">
        <template #icon><delete-two-tone /></template>
      </a-button>
    </a-divider>
  </div>
</template>

<style lang="scss">
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