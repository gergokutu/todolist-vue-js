<template>
  <div id="app">
    <Header />
    <router-view/>
    <div class="links">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  </div>
</template>

<script>
import Header from './components/layouts/Header';

export default {
  name:"app",
  components: {
    Header
  }
}
</script>


<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }
  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }
  .btn:hover {
    background: #666;
  }

  .links {
    text-align: center;
    margin: 5px;
  }
</style>