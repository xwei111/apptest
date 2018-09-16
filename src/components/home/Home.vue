<template>
	<div class='main'>
		<ViewBox>
			<swiper loop auto :list="demo06_list" :index="demo06_index" @on-index-change="demo06_onIndexChange"></swiper>
		</ViewBox>
	</div>
</template>
<script>
	import { Swiper,ViewBox } from 'vux'

	const baseList = [{
	  url: 'javascript:',
	  img: 'https://ww1.sinaimg.cn/large/663d3650gy1fq66vvsr72j20p00gogo2.jpg',
	  title: '送你一朵fua'
	}, {
	  url: 'javascript:',
	  img: 'https://ww1.sinaimg.cn/large/663d3650gy1fq66vw1k2wj20p00goq7n.jpg',
	  title: '送你一辆车'
	}, {
	  url: 'javascript:',
	  img: 'https://static.vux.li/demo/5.jpg', // 404
	  title: '送你一次旅行',
	  fallbackImg: 'https://ww1.sinaimg.cn/large/663d3650gy1fq66vw50iwj20ff0aaaci.jpg'
	}]

	const urlList = baseList.map((item, index) => ({
			  url: 'http://m.baidu.com',
			  img: item.img,
			  fallbackImg: item.fallbackImg,
			  title: `(可点击)${item.title}`
			}))

	export default{
		name:'Home',
		components: {
		    Swiper,
		    ViewBox
		},
		data(){
			return {
				demo06_list:urlList,
				demo06_index:0,
			}
		},
		methods:{
			demo06_onIndexChange(index){
				alert(index)
			}
		}
	}
</script>
<style scoped>

</style>