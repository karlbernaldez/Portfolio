<template>
  <header class="site-header">
    <nav class="navbar">
      <div class="container d-flex justify-content-between align-items-center">
        <ul class="navbar-nav d-flex flex-row">
          <li class="nav-item">
            <router-link to="/about" class="nav-link-home">Home</router-link>
          </li>
          <li class="nav-item">
            <a href="#about" class="nav-link">About</a>
          </li>
          <li class="nav-item">
            <router-link to="/contact" class="nav-link">Portfolio</router-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  // No specific JavaScript logic needed
}
</script>

<style scoped>

</style>
