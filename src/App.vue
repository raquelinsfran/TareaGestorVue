<template>
  <div id="app">
    <!-- Barra de navegación con enlaces a diferentes rutas -->

    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/">Home</router-link> |
            </li>
            <li class="nav-item">
              <router-link to="/addtask">Agregar Tarea</router-link> |
            </li>
            <li class="nav-item">
              <router-link to="/tasklist">Lista de Tareas</router-link> |
            </li>
            <li class="nav-item">
              <router-link to="/combinedview">Vista Combinada</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>





    <!-- Aquí se cargará el componente correspondiente a la ruta seleccionada -->
    <router-view />
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

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
