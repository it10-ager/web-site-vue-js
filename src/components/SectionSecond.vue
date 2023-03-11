<template>
	<section id="second-section">
		<!--------------------------------------------1-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale1" src="../img/Difficult-lang1.jpeg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale1)" v-on:mouseout="noscaleImg($refs.imgscale1)">
			</div>
			<div class="news-txt">
				<p>Какие языки программирования ненавидят больше и почему?</p>
				<p>
					Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении
					языков программирования. В этот раз в центре внимания нелюбимые языки.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------2-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale2" src="../img/Camera1.jpg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale2)" v-on:mouseout="noscaleImg($refs.imgscale2)">
			</div>
			<div class="news-txt">
				<p>Надо ли заклеивать камеру на ноутбуке?</p>
				<p>
					Заклеивать камеру ноутбука - паранойя или эффективное средство защититься от хакеров?
					Мы рассмотрим аспекты за и против и ответим на этот вездесущий вопрос.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------3-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale3" src="../img/Future1.jpg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale3)" v-on:mouseout="noscaleImg($refs.imgscale3)">
			</div>
			<div class="news-txt">
				<p>5 будущих профессий для IT специалистов</p>
				<p>
					Профессии постоянно пополняются и IT сфера вовсе не исключение.
					Мы подготовили список из 5 возможнных будущих профессий, к которым можно
					подготовиться уже сейчас.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------4-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale4" src="../img/Python1.jpg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale4)" v-on:mouseout="noscaleImg($refs.imgscale4)">
			</div>
			<div class="news-txt">
				<p>ИИ на Python для распознавания голоса</p>
				<p>
					На Python можно строить как простые программы, так и сложные
					ИИ системы. В данной статье мы покажем как реализовать распознавание
					голоса и выполнение различных команд.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------5-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale5" src="../img/Git1.jpg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale5)" v-on:mouseout="noscaleImg($refs.imgscale5)">
			</div>
			<div class="news-txt">
				<p>Изучение Git на реальных примерах</p>
				<p>
					Git - это очень полезная система управления версиями, которая позволяет
					разработчикам эффективнее работать вместе. В статье вкратце на примерах,
					вы изучите основные моменты Git.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------6-------------------------------------------->
		<div class="news-list">
			<div class="news-img">
				<img ref="imgscale6" src="../img/Javascript1.jpg" alt="photo-google" v-on:mouseover="scaleImg($refs.imgscale6)" v-on:mouseout="noscaleImg($refs.imgscale6)">
			</div>
			<div class="news-txt">
				<p>Почему JavaScript очень крутой язык программирования?</p>
				<p>
					Язык JavaScript за последние года стал мега популярным и завоевал
					огромное доверие среди разработчиков. Почему он так крут?
					Узнаем в этой статье.
				</p>
			</div>
			<div class="news-btn">
				<button>Далее</button>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
 		methods: {
			scaleImg(img) {
				img.style.transform = "scale(1.1)";
			},
			noscaleImg(img) {
				img.style.transform = "scale(1)";
			},
		},
	};
</script>

<style scoped lang="scss">

</style>