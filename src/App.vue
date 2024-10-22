<template>
  <div id="app" class="d-flex">
    <!-- Sidebar -->
    <div :class="['sidebar', { collapsed: isSidebarCollapsed }]">
      <button class="btn btn-primary mt-3" @click="toggleSidebar">
        <i class="fas" :class="isSidebarCollapsed ? 'fa-bars' : 'fa-times'"></i>
      </button>
      <ul class="nav flex-column mt-3">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Services</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>

    <!-- Main content -->
    <div class="main-content">
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">My App</a>
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
              <a class="nav-link active" href="#">Dashboard</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Profile</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Settings</a>
            </li>
          </ul>
        </div>
      </nav>

      <div class="container mt-4">
        <h1>Welcome to My App</h1>
        <p>This is a collapsible sidebar layout built with Vue 3 and Bootstrap 5.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isSidebarCollapsed: false
    }
  },
  methods: {
    toggleSidebar() {
      this.isSidebarCollapsed = !this.isSidebarCollapsed
    }
  }
}
</script>

<style scoped>
/* Sidebar styles */
.sidebar {
  width: 250px;
  height: 100vh;
  background-color: #343a40;
  padding: 15px;
  transition: width 0.3s ease;
}

.sidebar.collapsed {
  width: 80px;
}

.sidebar .btn {
  width: 100%;
}

.sidebar ul {
  margin-top: 20px;
}

.sidebar .nav-link {
  color: #fff;
  padding: 10px 15px;
}

.sidebar .nav-link:hover {
  background-color: #495057;
}

.sidebar.collapsed .nav-link {
  text-align: center;
  padding: 10px;
  font-size: 0;
}

.sidebar.collapsed .nav-link::before {
  font-size: 1.2rem;
}

.sidebar .nav-link.active {
  background-color: #495057;
}

/* Main content */
.main-content {
  flex-grow: 1;
}

.navbar {
  z-index: 1000;
  width: 100%;
}
</style>
