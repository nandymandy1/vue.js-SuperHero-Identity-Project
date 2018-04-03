<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>

export default {
  data () {
    return {
      title:' Vue Super Heros'
    }
  },
  methods:{

  }
}
</script>

<style scoped>
  header{
    background: #2E86C1;
    padding:10px;
  }
  h1{
    color:#fff;
    text-align: center;
  }
</style>
