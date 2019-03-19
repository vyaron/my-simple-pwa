<template>
  <div class="hello">
    <h1>{{ myMsg }}</h1>
    <button @click="addPower">Louder</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data () {
    return {
      myMsg: this.msg
    }
  },
  methods: {
    addPower () {
      this.myMsg += '!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
