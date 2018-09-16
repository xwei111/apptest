<template>
	<div >
		<Tabbar class='footer'>
			<TabbarItem selected link='/'>
				<span slot='label'>首页</span>
			</TabbarItem>
			<TabbarItem link='/detail'>
				<span slot='label'>详情</span>
			</TabbarItem>
			<TabbarItem link='/setInfo'>
				<span slot='label'>设置</span>
			</TabbarItem>
		</Tabbar>

	</div>
</template>
<script>
	import { Tabbar, TabbarItem } from 'vux'
	export default{
		name:'Footer',
		components: {
		    Tabbar,
		    TabbarItem
	    }
	}
</script>
<style scoped>
.footer{
	position: fixed;
	bottom: 0;
	left: 0;
}
</style>