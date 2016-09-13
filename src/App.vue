<template>
  <div id="app well">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import Pagination from './Pagination'

export default {
  data () {
    return {
      msg: 'Hello Vue!'
    }
  }
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
