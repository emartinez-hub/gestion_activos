<template>
  <nav
    class="navbar navbar-expand-md navbar-dark bg-dark border-bottom border-body px-3 px-md-5 d-md-none"
    data-bs-theme="dark"
  >
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Gestión Activos</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"
              ><i class="bi bi-speedometer2"></i> Dashboard</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><i class="bi bi-briefcase"></i> Operaciones</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><i class="bi bi-box-seam"></i> Paquetería</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><i class="bi bi-headset"></i> Servicio al Cliente</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="d-flex">
    <!-- Sidebar para

    pantallas grandes (md up) -->
    <div class="sidebar d-none d-md-block">
      <h4 class="te xt-light mb-4">Gestión Activos</h4>
      <a href="#"> <i class="bi bi-speedometer2 me-2"></i> Dashboard</a>
      <a href="#"><i class="bi bi-briefcase me-2"></i> Operaciones</a>
      <a href="#"><i class="bi bi-box-seam me-2"></i> Paquetería</a>
      <a href="#"><i class="bi bi-headset me-2"></i> Servicio al Cliente</a>
    </div>

    <!-- Contenido principal -->
    <div class="container mt-4 w-100">
      <h1>Welcome to My App</h1>
      <p>This is a collapsible sidebar layout built with Bootstrap 5.</p>
    </div>
  </div>
</template>

<script lang="ts"></script>

<style scoped>
.sidebar {
  width: 250px;
  min-height: 100vh;
  background-color: #343a40;
  padding: 15px;
}

.sidebar a {
  color: #fff;
  text-decoration: none;
  margin-bottom: 15px;
  display: block;
}
</style>
