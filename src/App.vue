<template>
	<div id="app-wrapper">
		<TheHeader />
		<TheMain />
		<TheFooter />
	</div>
</template>

<script setup lang="ts">
import { onMounted } from 'vue' // 1. 마운트될 때 실행하려고 가져옴!
import axios from 'axios'        // 2. 통신 도구 가져옴!

// 만든 컴포넌트들을 가져오는 거야!
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'

// 3. 페이지가 딱 켜지자마자 실행되는 함수!
onMounted(() => {
	axios.get('http://localhost:8080/api/test')
			.then(res => {
				// 이제 알림창 대신 콘솔로만 조용히 확인! 😎
				console.log("DB에서 온 소중한 데이터들:", res.data);
			})
			.catch(err => {
				console.error("데이터 가져오기 실패ㅠ:", err);
			});
})
</script>

<style lang="scss">
/* 전역 스타일이나 레이아웃 설정 */
#app-wrapper {
	display: flex;
	flex-direction: column;
	min-height: 100vh;
}
</style>