<template>
	<div class="container-menu">
		<div class="search">
			<input type="text" name="name" placeholder="Поиск" autocomplete="off">
		</div>

		<div>
			<div class="nav-txt">
				<p>Меню</p>
				<span class="blue-line-half"></span>
			</div>

			<div class="navigation">
				<p>Главная</p>
				<p>Про нас</p>
				<p>Контакты</p>
			</div>

			<div class="info-about">
				<p>Информация про нас</p>
				<span class="blue-line-half"></span>
			</div>

			<div class="info-new">
				<div class="info-img" ref="scale1" v-on:mouseover="scaleSize($refs.scale1)" v-on:mouseout="defaultScale($refs.scale1)">
					<img src="../img/kotik.jpg" alt="photo-kotik">
				</div>
				<div class="info-txt">
					<p>
						На днях был придуман новый язык программирования - Kotik!
					</p>
				</div>
			</div>

			<div class="info-new" style="border-bottom: none;">
				<div class="info-img" ref="scale2" v-on:mouseover="scaleSize($refs.scale2)" v-on:mouseout="defaultScale($refs.scale2)">
					<img src="../img/apple.jpg" alt="photo-apple">
				</div>
				<div class="info-txt">
					<p>
						Эксперты усомнились в подлинности данных, которые предоставила
						компания Apple.
					</p>
				</div>
				<div class="info-btn">
					<button>Далее</button>
				</div>
			</div>

			<div class="help">
				<p>Помощь</p>
				<span class="blue-line-half"></span>
			</div>

			<div class="help-txt">
				<p>
					Если у вас возникли какие-либо вопросы и вы хотите
					связаться с нами для уточнения всех моментов, то ниже 
					представлены все контактные данные для связи с нами.
				</p>
			</div>

			<div class="help-contacts">
				<div>
					<img src="../img/message-envelope.png" alt="photo">
					<span>test@itproger.com</span>
				</div>
				<div>
					<img src="../img/call-answer (1).png" alt="photo">
					<span>(000) 000 - 0000</span>
				</div>
				<div>
					<img src="../img/home.png" alt="photo">
					<span>USA Washington Seatles Northway 13002</span>
				</div>
			</div>

			<div class="policy">
				<span>
					Все права защищены &copy;. При использовании
					данных указывайте ссылку на первоисточник.
				</span>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
 		methods: {
			scaleSize(img) {
				img.style.transform = "scale(1.02)";
			},
			defaultScale(img) {
				img.style.transform = "scale(1)";
			},
		},
	};
</script>

<style scoped lang="scss">
	@import '../assets/main.menu.scss';
</style>