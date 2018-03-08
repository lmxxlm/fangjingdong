<template lang="html">
	<Panel title="金融头条" :class="$style.panel">
		<section :class="$style.content">
            <swiper :options="options">
            	<swiper-slide>随便测试1</swiper-slide>
            	<swiper-slide>随便测试3</swiper-slide>
            	<swiper-slide>解决的恢复精神负担和 <em>></em></swiper-slide>
            	<swiper-slide>好地方还是干活 <em>></em></swiper-slide>
            </swiper>
		</section>
	</Panel>
</template>
<script>
	import Panel from '../core/panel.vue'
	import {swiper,swiperSlide} from "vue-awesome-swiper"
	export default{
		components:{
			Panel,
			swiper,
			swiperSlide
		},
		data(){
			return{
				options:{
					autoplay:true,
					loop:true,
					direction:"vertical"
				}
			}
		}
	}
</script>
<style lang="scss">
	.swiper-container-vertical{
		height:72px;
		.swiper-slide{
			font-family: PingFangSC-Medium;
			font-size:28px;
			color:#333;
			em{
				color:#ddd;
				float:right;
				margin-right:10px;
			}
		}
	}
</style>
<style lang="scss" module>
	@import '../../css/element.scss';
	.panel{
		@include panel;
		>h4{
			display:none;
		}
		margin-top:120px!important;
        .content{
        	height:72px;
        	line-height:72px;
        	overflow:hidden;
        	padding-left:146px;
        	background:url(//m.jr.jd.com/spe/qyy/main/images/scroll_title_img.png) left no-repeat;
        }
	}
</style>