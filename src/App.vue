<template>
  <div id="nav">
    <app-header />
    <router-view />
  </div>
</template>

<script>
import appHeader from '@/components/app-header'

export default {
  components: {appHeader}
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

html {
  font-size: 10px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.article {
  font-size: 1.4rem;
  padding: 2rem;
  &__header {
    font-size: 2rem;
    font-weight: 500;
    padding: 2rem 0;
  }
}
</style>
