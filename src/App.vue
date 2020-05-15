<template>
  <div id="app">
    <ul id="menu">
        <li data-menuanchor="firstPage" class="active"><a href="#firstPage">First section</a></li>
        <li data-menuanchor="secondPage"><a href="#secondPage">Second section</a></li>
        <li data-menuanchor="thirdPage"><a href="#thirdPage">Third section</a></li>
      </ul>
    <full-page ref="fullpage" :options="options" id="fullpage">
      <div class="section">
        <img src="./assets/images/vietnam.jpg" alt="">
      </div>
      <div class="section">
        <img src="./assets/images/vietnam2.jpg" alt="">
      </div>
      <div class="section">
        <img src="./assets/images/vietnam3.jpg" alt="">
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
          anchors: ['firstPage', 'secondPage', 'thirdPage'],
          sectionsColor: ['#41b883', '#ff5f45', '#0798ec'],
          menu: '#menu'
        }
      }
    }
  }
</script>

<style>
  a {
    text-decoration: none;
  }
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    /* margin-top: 60px; */
  }
  #menu {
    position: absolute;
    top: 1px;
    right: 1px;
    z-index: 70;
  }
  #menu li {
    display: inline-block;
    margin: 10px 0;
    position: relative;
  }
  #menu li a {
    color: #fff;
    padding: 0 1.1em 1.1em 1.1em;
  }
  #menu li.active a:after {
    content: '';
    margin: 0 1.1em 0 1.1em;
    height: 2px;
    background: #fff;
    display: block;
    position: absolute;
    bottom: -6px;
    left: 0;
    right: 0;
    display: block;
  }
</style>
