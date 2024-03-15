<template>
	<el-card shadow="never">
		<sc-statistic title="统计" :value="count" suffix="个" groupSeparator>
			<sc-trend v-model="trend"></sc-trend>
		</sc-statistic>
	</el-card>
</template>

<script>
import scStatistic from "@/components/scStatistic";

export default {
	name: "device-dashboard",
	title: "网络组件",
	icon: "el-icon-clock",
	description: "网络组件模块",
	components: {
		scStatistic
	},
	data() {
		return {
			count: 0,
			trend: 0
		}
	},
	mounted() {
		this.initDashboard()
	},
	methods: {
		async initDashboard() {
		},
	}
}
</script>

<style scoped>

</style>
