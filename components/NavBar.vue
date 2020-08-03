<template>
  <header>
    <div class="container">
      <nav>
        <nuxt-link to="/">Index</nuxt-link>
        <nuxt-link to="/about">About</nuxt-link>
        <nuxt-link to="/list">List</nuxt-link>
      </nav>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
header {
  padding: 2rem;
  background-color: lightcoral;
}
nav {
  float: right;
}
a,
a:visited {
  text-decoration: none;
  padding: 1rem;
}
</style>