<template>
  <app-header />
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <Main msg="Welcome to Your Vue.js + TypeScript App"/>
  <app-footer />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'
import Main from './components/Main.vue'
import AppHeader from '@/components/AppHeader.vue'
import AppFooter from '@/components/AppFooter.vue'

@Options({
  components: {
    Main,
    AppHeader,
    AppFooter
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
$primary: #FBFBFB;
$primary-opacity-70: #fbfbfbab;
$primary-opacity-50: #fbfbfb7a;
$primary-dark: #080707;
$second: #F3A712;
$second-opacity: #0710138a;
$second-dark: #071013;

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body{
  background: $primary;
  margin: 0;
}

.page{
  background: $primary;
  margin: 0;
  padding: 3.5em 0;
  box-shadow: 0 0.2em 0.5em $second-opacity;
}

header{
  display: flex;
  position: fixed;
  top: 0;
  width: 100%;
  height: 3em;
  background: $second;
  a {
    font-weight: bold;
    color: $primary-opacity-70;
    text-decoration: none;
  }
  a:hover{
    color:$primary-dark;
  }
  p {
    margin-left: 1rem;
  }
  box-shadow: 0px 0px 1em $second-opacity;
}

footer {
  background: $second-dark;
  padding: 5em 2em 4em 2em;
  margin: 0;
}

.top-border {
  border-top: 1px solid $primary-opacity-50;
}

.color-primary-80{
  color: $primary;
  opacity: 0.7;
}

nav {
    margin-left: 1em;

    ul {
      list-style: none;
    }

    ul li {
      display: inline-flex;
      margin-left: 1rem;
    }
}

.inner{
  padding: 3em;
}

.orange{
  background: $second;
  padding-bottom: 10em;
}

.white-card{
  background: $primary;
  border-radius: 12px;
  box-shadow: 0 5px 5px 0 $second-opacity;
  padding: 5em;
  z-index: 10;
}

.margin-minus{
  margin-top: -10em;
}

</style>
