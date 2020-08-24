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
                            <!-- <Search_Bar /> -->
                            <b-field>
                                <b-input name="location" v-model="location" @keyup.enter="say('Hi!')" placeholder="Type on me, baby!" size="is-large"></b-input>
                            </b-field>
                            <!-- <input v-model="location" placeholder="type here"> -->
                            <button v-on:click="say('hi')">Say hi</button>
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
/* import Search_Bar from './components/Search_Bar' */

export default {
  name: 'App',
  components: {
    /* Search_Bar */
  },
  data() {
      return {
          location: ''
      }
  },
  methods: {
    say: function (message) {
      alert(message)
    }
  }
}
</script>

<style>

</style>
