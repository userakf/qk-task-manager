<template>
  <Header />
  <div class="conatiner">
    <div class="header">
      <div class="text">
        <p>Excellence management</p>
        <span>Lorem ipsum dolor sit amet</span>
      </div>
      <div class="icon">
        <Icon size="20" type="info"/>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import './index.scss'
import Header from '../../components/header/index.vue'
import { Icon } from '@tarojs/components';
</script>
<style lang="scss">
.conatiner{
  padding: 30px 60px;
}
</style>