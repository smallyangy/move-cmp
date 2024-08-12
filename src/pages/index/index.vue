<template>
	<view>
		我是主页
		<button @click="handleGo('/subpackages/pageA/index')">pageA</button>
		<button @click="handleGo('/subpackages/pageB/index')">pageB</button>
		<CMPA></CMPA>
	</view>
</template>

<script>
	import CMPA from '@/components/CMPA.vue'
	export default {
		components: {
			CMPA,
		},
		data() {
			return {}
		},
		methods: {
			handleGo(url) {
				uni.navigateTo({
					url
				})
			}
		}
	};
</script>

<style lang="scss">

</style>
