<template>
  <div id="app-wrapper">
    <TheHeader />
    <TheMain />
    <TheFooter />
  </div>
</template>

<script setup lang="ts">
// 만든 컴포넌트들을 가져오는 거야!
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'
</script>

<style lang="scss">
/* 전역 스타일이나 레이아웃 설정 */
#app-wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
</style>