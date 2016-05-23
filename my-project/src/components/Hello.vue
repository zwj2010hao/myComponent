<template>
    <img src="../assets/logo.png" width="499" height="100">
    <h1>There are some components that I collected .</h1>
</template>

<script>
export default {
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg:'a'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import "./style/hello.scss";
</style>
