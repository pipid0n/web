<template>
  <div id="app">
    <header class="header">
      <div class="container">
        <div class="header__inner">
          <div class="header__logo">Gunshop</div>

          <nav class="nav">
            <ul>
              <li>
                <router-link :to="{name: 'About'}">О нас</router-link>
              </li>
              <li>
                <router-link :to="{name: 'Catalog'}">Каталог</router-link>
              </li>
              <li>
                <router-link :to="{name: 'Stores'}">Наши салоны</router-link>
              </li>v
              <li>
                <router-link :to="{name: 'Shipping'}">Доставка</router-link>
              </li>
              <li>
                <router-link :to="{name: 'Contacts'}">Контакты</router-link>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
