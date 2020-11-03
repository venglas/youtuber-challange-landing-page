<template>
  <article class="article">
    <header class="article__header">
      Witaj na Youtuber Challange dev page!
    </header>
    <p>
      Ponizej znajdziesz informacje na temat projektu oraz niezbędne linki, które pomogą Ci szybciej podjąć decyzję czy chcesz mieć swój wkład w ten projekt.
    </p>

    <h4 style="margin: 3rem 0 1rem 0">Lista technologii uzytych w projekcie</h4>

    <div class="section-wrapper">
      <section class="article__section article__section--front-end">
      <header class="header">
        front-end
      </header>
      <ul class="list">
        <li class="list__item" v-for="technology in frontEndTechnologies" :key="technology">
          {{technology}}
        </li>
      </ul>
    </section>

    <section class="article__section article__section--front-end">
      <header class="header">
        back-end
      </header>
       <ul class="list">
        <li class="list__item" v-for="technology in backEndTechnologies" :key="technology">
          {{technology}}
        </li>
      </ul>
    </section>
    </div>

    <section class="article__section">
      <header class="header">
        Jak działamy?
      </header>
      <p>
        Wszystkie sprawy związane z projektem przechowywane są w jednym miejscu, a tym miejscem jest github. <br />
        Dokumentacja, tablice kanban, issues. <br />
        Wersjonowanie projektów oparte jest o <a href="https://semver.org/lang/pl/">semantyczne wersjonowanie</a>.
      </p>
    </section>

    <section class="article__section">
      <header class="header">
        Kto moze kontrybułować?
      </header>
      <p>
        Swój wkład w projekt moze mieć kazdy. Mniej lub bardziej doświadczony zawodnik. <br />
        Aktualnie szukamy pomocy zarówno z front endu i back endu. <br />
        Nie negujemy nikogo, chcesz uczestniczyć w zarządzaniu projektem, słuyć swoją pomocą przy ux/ui designie, albo testach? <br />
        - To odpowieni projekt dla Ciebie :) <br />

        <span style="width: 100%; border-bottom: 1px solid gray; display: block; margin: 1rem"></span>

        Jeśli jesteś zainteresowany dołącz do discorda, a otrzymasz więcej informacji:
        <a href="https://discord.gg/JUv3va2y" target="_blank">Kliknij tutaj aby odebrać zaproszenie</a>
      </p>
    </section>
  </article>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const frontEndTechnologies = ref([
      'pwa application',
      'nuxt',
      'composition api',
      'axios',
      'type-script'
    ])

    const backEndTechnologies = ref([
      'rest API',
      'node',
      'express',
      'type-script',
      'mongoose',
      'mongodb',
      'dotenv',
      'winston'
    ])

    return {
      frontEndTechnologies,
      backEndTechnologies
    }
  }
}
</script>

<style lang="scss">
.article {
  .section-wrapper {
    display: flex;
    justify-content: space-evenly;
  }
  &__section {
    margin: 1rem 0;
    .header {
      font-weight: 500;
      margin: .5rem 0;
    }
    &--front-end {
      font-size: 1.7rem;
    }
  }
  .list {
    text-align: left;
  }
}
</style>