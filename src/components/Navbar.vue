<template>
  <div id="navbar" class="navbar">
    <div class="container">
      <router-link to="/">Home</router-link>
      <router-link to="/portfolio">Portfolio</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({ })
export default class Home extends Vue {}
</script>

<style scoped>
#navbar {
  padding: 20px;
  display: flex;
  justify-content: center;
}

.container {
  width: 25%;
  height: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.container a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}
.container a.router-link-exact-active {
  color: #42b983;
}
</style>
