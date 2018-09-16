<template>
	
		<x-header :left-options='obj' title='Test'/>
	
</template>
<script>
	export default{
		name:'Header',
		data(){
			return {
				obj:{
					showBack:false
				}
			}
		}
	}
</script>
<style scoped>

</style>