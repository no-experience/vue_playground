<template>
  <div id="app">
    <body>
		<section class="section">
			<div class="container">
				<div class="columns is-centered">
					<h1 class="title is-1">Vue Playground!</h1>
				</div>
			</div>
		</section>
    </body>
  </div>
</template>

<script>
// Standard Imports
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'

// Imports de componentes
import Search_Bar from './components/Search_Bar'

Vue.use(Buefy)

export default {
  name: 'App',
  components: {
    Search_Bar
  }
}
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }
</style>
