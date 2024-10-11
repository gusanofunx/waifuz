<template>
  <nav class="     bg-black  py-2 px-3">
    <div class=" flex justify-between">
      <a class="navbar-brand" href="#">Only Waifus</a>

      <div class="     text-white" id="navbarSupportedContent">
        <ul class=" flex text-white">
          <li class=" text-white  ">
            <router-link class="nav-link" to="/">Inicio</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Acerca de</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contacto</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>

</script>

<style scoped>
.navbar {
  padding: 1rem;
  background-color: #f8f9fa;
  border-bottom: 1px solid #dee2e6;
}

.navbar-brand {
  color: rgb(252, 203, 179);
  font-weight: bold;
  font-size: 1.5rem;
}

.nav-link {
  color: #333;
  transition: color 0.2s ease;
}

.nav-link:hover {
  color: #337ab7;
}
</style>
