<template>
  <Menu/>
  <Form/>
</template>

<script>
import Menu from "./components/MenuBar.vue"
import Form from "./components/FormView.vue"
export default {
  components: {
    Menu,
    Form
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
