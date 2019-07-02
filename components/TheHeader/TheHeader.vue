<template>
  <header class="main-header">
    <logo />
    <nav class="main-nav">
      <ul class="nav-links">
        <nuxt-link to="/" class="nav-link" tag="li"><a>All Posts</a></nuxt-link>
        <nuxt-link to="/about" class="nav-link" tag="li"
          ><a>About</a></nuxt-link
        >
      </ul>
    </nav>
  </header>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style scoped>
.main-header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #022d30;
  height: 5.5rem;
}

.main-nav {
  height: 100%;
}
.nav-links {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
}
.nav-link {
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0.1rem;
  padding: 0.3rem;
  border-bottom: 10px solid transparent;
}
.nav-link a {
  display: block;
  text-decoration: none;
  color: white;
}

.nav-link.nuxt-link-exact-active {
  border-bottom: 10px solid #06c4d1;
}

.nav-link a:hover,
.nav-link a:active,
.nav-link.nuxt-link-exact-active a {
  color: #06c4d1;
}
</style>
