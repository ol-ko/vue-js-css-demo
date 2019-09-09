<template>
  <div id="app">
    <section>
      <BlackCircle text="Black circle"/>
      <RedRombus text="Red rombus"/>
      <section class="context">
        <BlackCircle text="Black circle" :cssClass="$style.inverted"/>
      </section>
    </section>
  </div>
</template>

<script>
import BlackCircle from './components/BlackCircle.vue'
import RedRombus from './components/RedRombus.vue'

export default {
  name: 'app',
  components: {
    BlackCircle,
    RedRombus
  }
}
</script>

<style>
  body {
    margin: 0;
    padding: 0;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  section {
    display: flex;
    justify-content: center;
    padding: 20px;
  }

  .context {
    background: black;
  }
</style>

<style lang="scss" module>
  .inverted {
    background: white;
    color: black;
  }
</style>
