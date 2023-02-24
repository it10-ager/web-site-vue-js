<template>
	<MenuBlock />

	<div class="container">
		<div class="menu-icon">
			<img class="button-menu" src="./img/menu icon.png" alt="menu-icon" @click="changePosition">
		</div>
		<header>
			<span>СМИ портал</span>
			<span class="blue-line"></span>
		</header>

		<SectionFirst />

		<div class="last-published">
			<p>Последние опубликованные</p>
			<span class="blue-line-half"></span>
		</div>
		
		<SectionSecond />

		<SectionThird />

		<div class="info">
			<p>Информация</p>
			<span class="blue-line-half"></span>
		</div>

		<footer>
			<!--------------------------------------------1-------------------------------------------->
			<div>
				<div class="footer-img">
					<img src="./img/multiple-users-silhouette icon.png" alt="user">
				</div>
				<div class="footer-txt">
					<p>Множество клиентов</p>
					<p>
						Огромное количество клиентов выбирают нас, так как мы всегда
						держим руку на пульсе всего происходящего
					</p>
				</div>
			</div>
			<!--------------------------------------------2-------------------------------------------->
			<div>
				<div class="footer-img">
					<img src="./img/youtube icon.png" alt="yt">
				</div>
				<div class="footer-txt">
					<p>Большая аудитория YouTube</p>
					<p>
						Большая фан база на площадке YouTube. Вы всегда сможете
						найти ту информацию, которая сейчас у всех на слуху на нашем канале
					</p>
				</div>
			</div>
		</footer>
	</div>
</template>

<script>
	import SectionFirst from './components/SectionFirst.vue';
	import SectionSecond from './components/SectionSecond.vue';
	import SectionThird from './components/SectionThird.vue';
	import MenuBlock from './components/MenuBlock.vue';

	export default{
		components: {
			SectionFirst,
			SectionSecond,
			SectionThird,
			MenuBlock,
		},

		data(){
			return{
				isPositioned: false,
			};
		},

		methods:{
			changePosition() {
				var container = document.querySelector(".container");
				var containerMenu = document.querySelector(".container-menu");
				this.isPositioned = !this.isPositioned; 

				if (this.isPositioned){
					container.classList.remove("position-change");
					containerMenu.classList.remove("position-change-menu");
					container.classList.add("position");
					containerMenu.classList.add("position-menu");
				}
				else {
					containerMenu.classList.remove("position-change-menu");
					container.classList.remove("position");
					containerMenu.classList.remove("position-menu");
					container.classList.add("position-change");
					containerMenu.classList.add("position-change-menu");
				}
			},
		},
	};
</script>

<style lang="scss">
	@import './assets/main.scss';
</style>