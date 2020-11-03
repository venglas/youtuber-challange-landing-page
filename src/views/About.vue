<template>
  <article class="article">
    <header class="article__header">
      Apka? Ale jaka apka?
    </header>
    <p>
      Jak wiadomo jutuberzy to bestie na glinianych nogach i chętnie podejmią się wyzwań, które zaproponował im ich widz, który został poparty przez resztę publiczności więc
    </p>

    <h4 style="margin: 3rem 0 1rem 0">Więc stajemy naprzeciw i dajemy mozliwość rzucania wyzwań :)</h4>

    <section class="article__section">
      <header class="header">
        Koncepcja
      </header>
      <p>
        Aplikacja ma dać uytkownikom mozliwość stworzenia wyznawania "challange'u" i przypisania go do danego Youtubera. Wyzwania będą się wyświetlać na stronie głównej najpopularniejsze, etc. z moliwością filtrowania. <br />
        Wyzwania akceptować będą mogli tylko youtuberzy do których kierowane jest dane wyzwanie.
      </p>
  </section>

  <section class="article__section">
    <header class="header">
      O projekcie w rzeczy samej
    </header>
    <p>
      Na aplikacjie składa się warstwa front-endu oparta o Nuxt z composition api, cały stack moesz zobaczyć <router-link to="/home">tutaj</router-link>, oraz warstwa back-endu oparta o node + express, cały stac równiez zobaczysz pod wcześcniej wymienionym linkiem. <br />
      Projekt jest w początkowej fazie rozwoju. Co to oznacza? <br />
      Oznacz to mniej więcej to, ze kazda osoba ma wplyw na to jak finalnie produkt bedzie sie prezentowal, jakie technologie zostana uzyte, jak beda dzialay poszczegolne ficzery, oraz wiele wiele innych. Projekt nie jest nastawiony na zarabianie, tylko na zbudowaniu fajnego grona przyjaznego rozwijaniu się, oraz wspólpracy :) <br />
      Finalnie potencjalne zyski z reklam przeznaczone będą na rozwiój projektu oraz utrzymanie jego serwerów.
    </p>
  </section>

  <h4 style="margin: 3rem 0 1rem 0">Zainteresowany? Dołącz do nas na discordzie i stań się członkiem ekipy 
    <a href="https://discord.gg/JUv3va2y" target="_blank">Kliknij tutaj aby odebrać zaproszenie</a>
  </h4>
  </article>
</template>


<style lang="scss" scoped>
  .article {
    &__section {
      margin: 3rem 0;
    }
  }
</style>