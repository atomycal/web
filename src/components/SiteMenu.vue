<script setup>
import { ref, computed } from 'vue'

const isShowOverlay = ref(false)
const overlayDisplay = computed(() => isShowOverlay.value === true ? 'block' : 'none')

const siteMenuItems = ref([
	{
		name: 'Home',
		to: '/'
	},

	{
		name: 'Portfolio',
		to: '/portfolio'
	},

	{
		name: 'Services',
		to: '/services'
	},

	{
		name: 'Contact Us',
		to: '/contact-us'
	}
])
</script>

<template>
	<header class="am-header" role="header">
		<div class="am-overlay"></div>

		<div class="am-nav-main">
			<div class="am-sale-main">
				<a class="button" href="#">-</a>
			</div>

			<div class="am-brand-main">-</div>

			<div class="am-menu-main">-</div>
		</div>
	</header>
</template>

<style scoped lang="scss">
.am-header {
	z-index: 5000;
	background-color: #000;
}

.am-overlay {
	position: fixed;
	left: 0;
	right: 0;
	top: 0;
	bottom: 0;
	background-color: rgba(0, 0, 0, 0.8);
	display: v-bind(overlayDisplay);
}

.am-nav-main {
	display: flex;
	justify-content: space-between;

	color: white;
	padding: 1rem;
}

.am-sale-main {
	.button {
		text-decoration: none;

		background-color: #AABD8C;
		color: #191308;
		padding: .5rem 1rem;
		border-radius: .25rem;
	}
}
</style>