<template>
  <div class="">
    <app-header></app-header>
    <app-heroes></app-heroes>
    <app-footer></app-footer>
  </div>

</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Heroes from './components/Heroes.vue'

export default {
  components:{
    'app-header': Header,
    'app-footer': Footer,
    'app-heroes': Heroes
  },
  name: 'app',
  data () {
    return {

    }
  },
  methods:{

  }
}
</script>

<style>

</style>
