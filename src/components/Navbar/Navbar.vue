<template>
  <div>
    <!-- Modern Sidebar -->
    <div class="sidebar">
      <router-link to="/" class="brand">
        <span>Tech Learn</span>
      </router-link>
      <ul class="nav flex-column">
        <li class="nav-item">
          <router-link
            to="/dashboard"
            class="nav-link"
            active-class="active"
            exact
          >
            <i class="bi bi-house-door-fill"></i> Dashboard
          </router-link>
        </li>
        <li class="nav-item">
          <router-link to="/" class="nav-link" active-class="active" exact>
            <i class="bi bi-house-door-fill"></i> Trang chủ
          </router-link>
        </li>
        <li class="nav-item">
          <router-link
            to="/profile"
            class="nav-link"
            active-class="active"
            exact
          >
            <i class="bi bi-person-circle"></i> Đăng xuất
          </router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
/* Sidebar styling */
.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 280px;
  height: 100vh;
  padding: 20px;
  background: linear-gradient(
    145deg,
    #2c3e50,
    #1a252f
  ); /* Gradient for modern effect */
  color: #ecf0f1;
  box-shadow: 2px 0 12px rgba(0, 0, 0, 0.2); /* Softer shadow */
  overflow-y: auto;
  transition: all 0.3s ease;
}

.brand {
  display: flex;
  align-items: center;
  margin-bottom: 30px;
  font-size: 1.8rem; /* Slightly larger logo text */
  color: #ecf0f1;
  text-decoration: none;
  font-weight: bold; /* Bold for logo */
  transition: color 0.3s ease;
}

.brand:hover {
  color: #3498db; /* Hover effect on logo */
}

.nav-link {
  display: flex;
  align-items: center;
  padding: 12px 15px;
  color: #ecf0f1;
  text-decoration: none;
  transition: background 0.3s ease, color 0.3s ease;
  border-radius: 8px;
  margin-bottom: 10px;
  font-weight: 500; /* More readable font */
}

.nav-link i {
  margin-right: 12px; /* Increase space between icon and text */
  font-size: 1.2rem; /* Larger icon */
  transition: transform 0.3s ease, color 0.3s ease; /* Smooth transition for hover effect */
}

.nav-link:hover i {
  transform: scale(1.1); /* Slight zoom effect on icon hover */
  color: #ecf0f1; /* Keep icon color on hover */
}

.nav-link:hover {
  background-color: #3498db;
  color: white;
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.15); /* Shadow for hover */
}

.nav-link.active {
  background-color: #2980b9;
  color: white;
  border-left: 4px solid #3498db; /* Highlight active link with left border */
}

.user-dropdown {
  margin-top: auto;
}

.user-info {
  display: flex;
  align-items: center;
  color: #ecf0f1;
  text-decoration: none;
  margin-bottom: 10px;
}

.user-info:hover {
  color: #3498db;
}

.user-img {
  margin-right: 10px;
}

.dropdown-menu {
  background-color: #34495e;
  color: #ecf0f1;
  border: none;
  padding: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  display: none;
}

.user-dropdown:hover .dropdown-menu {
  display: block;
}

.dropdown-item {
  color: #ecf0f1;
  padding: 5px 10px;
}

.dropdown-item:hover {
  background-color: #3498db;
  border-radius: 5px;
}
</style>
