<template>
  <header class="app-header">
    <nav class="app-header__nav">
      <ul class="menu">
        <li
          v-for="{ name, path } in routes"
          :key="name"
          class="menu__item"
        >
          <router-link :to="path">{{name}}</router-link>
        </li>
      </ul>
    </nav>
  </header>  
</template>

<script>
import { ref, onMounted } from 'vue'
import { useRouter } from 'vue-router'
export default {
  setup(_, context) {
    const routes = useRouter().getRoutes()
    
    onMounted (() => {
      console.log(routes)
    })

    return {
      routes
    }
  }
}
</script>

<style lang="scss">
  .app-header {
    font-size: 1.5rem;
    font-weight: 500;
    border-bottom: 1px solid lighten(#2c3e50, 40%);
    &__nav {
      display: flex;
      justify-content: flex-end;
      .menu {
        list-style-type: none;
        display: flex;
        width: fit-content;
        &__item {
          padding: 2rem;
        }
      }
    }
  }
</style>