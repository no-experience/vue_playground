<template>
    <b-field>
        <b-input name="location" v-model="location" placeholder="Type on me, baby!" size="is-large"></b-input>
    </b-field>
</template>

<script>
// Standard imports
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'
Vue.use(Buefy)

export default {
    name: 'Search_Bar',
    props: {
        /* location: location */
    },
    data(){ 
        return {
            location: ''
        };        
    }
}
</script>

