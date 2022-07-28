<template>
  <nav class="navbar navbar-expand-lg bg-danger bg-opacity-75">
    <div class="container-fluid">
      <nuxt-link class="navbar-brand" :to="'/'">Home</nuxt-link>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <nuxt-link :to="'/event'" class="nav-link">Event</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="'/asset'" class="nav-link">Asset</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="'/people'" class="nav-link">People</nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style>
</style>