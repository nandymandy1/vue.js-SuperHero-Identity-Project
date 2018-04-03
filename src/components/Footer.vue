<template>
  <footer>
    <p>{{ copyright }}</p>
  </footer>
</template>

<script>

export default {
  data () {
    return {
      copyright: 'Copyright @ 2018 Nandy Mandy'
    }
  },
  methods:{

  }
}
</script>

<style scoped>
footer{
  background: #2E86C1;
  padding: 6px;
}
p{
  color: #fff;
  text-align: center;
}
</style>
