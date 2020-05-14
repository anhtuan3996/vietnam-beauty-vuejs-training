<template>
  <div id="app">
    <full-page ref="fullpage" :options="options" id="fullpage">
      <div class="section">
        <img src="./assets/images/vietnam.jpg" alt="">
      </div>
      <div class="section">
        <img src="./assets/images/vietnam2.jpg" alt="">
      </div>
    </full-page>
  </div>
</template>

<script>

  export default {
    name: 'App',
    data() {
      return {
        options: {
          licenseKey: 'JDF8XRD6-JDF8XRD6-JDF8XRD6-JDF8XRD6',
          sectionsColor: ['#41b883', '#ff5f45', '#0798ec']
        }
      }
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
