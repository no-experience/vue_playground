<template>
  <div id="app">
	<body>
		<section class="hero is-fullheight is-light is-bold">
			<div class="hero-body">
				<div class="container">
					<div class="columns is-multiline is-mobile">
						<div class="column is-half">
							<h1 class="title is-3">What's the weather like in:</h1>
							<h2 id="" class="subtitle is-2">{{ location }}</h2>
						</div>
						<div class="column is-half">
							<Search_Bar />
						</div>
					</div>
				</div>
			</div>
		</section>
	</body>
  </div>
</template>

<script>
// Standard imports
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'
Vue.use(Buefy)

// Imports de componentes
import Search_Bar from './components/Search_Bar'

export default {
  name: 'App',
  components: {
	Search_Bar
  }
}
</script>

<style>

</style>
