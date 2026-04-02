<template>
	<header class="header">
		<div class="logo">LOGO</div>
		<nav>
			<ul>
				<li>메뉴1</li>
				<li>메뉴2</li>
			</ul>
		</nav>
		<button class="login-btn">로그인</button>
	</header>
</template>

<style lang="scss" scoped>
.header {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 1rem 2rem;
	background: #fff;
	border-bottom: 1px solid #eee;
	ul {
		display: flex;
		gap: 20px;
		list-style: none;
	}
}
</style>