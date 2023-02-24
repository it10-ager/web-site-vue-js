<template>
	<section id="third-section">
		<!--------------------------------------------1-------------------------------------------->
		<div class="another-news">
			<div class="another-img" v-on:mouseover="shadowBox" v-on:mouseout="defaultBlock">
				<img src="../img/frontend.png" alt="photo-google">
			</div>
			<div class="another-txt">
				<p>Front-end</p>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae, id minima.
				</p>
			</div>
			<div class="another-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------2-------------------------------------------->
		<div class="another-news">
			<div class="another-img" v-on:mouseover="shadowBox" v-on:mouseout="defaultBlock">
				<img src="../img/swift.jpg" alt="photo-google">
			</div>
			<div class="another-txt">
				<p>Swift</p>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae, id minima.
				</p>
			</div>
			<div class="another-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------3-------------------------------------------->
		<div class="another-news">
			<div class="another-img" v-on:mouseover="shadowBox" v-on:mouseout="defaultBlock">
				<img src="../img/V1.jpg" alt="photo-google">
			</div>
			<div class="another-txt">
				<p>Python</p>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae, id minima.
				</p>
			</div>
			<div class="another-btn">
				<button>Далее</button>
			</div>
		</div>
		<!--------------------------------------------4-------------------------------------------->
		<div class="another-news">
			<div class="another-img" v-on:mouseover="shadowBox" v-on:mouseout="defaultBlock">
				<img src="../img/angular.png" alt="photo-google">
			</div>
			<div class="another-txt">
				<p>Angular</p>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae, id minima.
				</p>
			</div>
			<div class="another-btn">
				<button>Далее</button>
			</div>
		</div>
	</section>
</template>

<script>
	export default{
		methods: {
			shadowBox(e) {
      			e.target.style.boxShadow = "0px 0px 20px 2px rgba(143,143,143,1)";
    		},
    		defaultBlock(e) {
     			e.target.style.boxShadow = "none";
    		},
 		},
	};
</script>

<style scoped lang="scss">

</style>