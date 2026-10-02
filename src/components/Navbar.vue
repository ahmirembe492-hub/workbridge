<template>
  <header class="navbar">
    <div class="container navbar-content">

      <a href="/" class="logo">
        WorkBridge
      </a>

      <nav class="nav-links">
        <a href="#">Find Jobs</a>
        <a href="#">Companies</a>
        <a href="#">Career Advice</a>
      </nav>

      <div class="nav-actions">
        <button class="login-button">
          Log in
        </button>

        <button class="signup-button">
          Sign up
        </button>
      </div>

    </div>
  </header>
</template>

<style scoped>
.navbar {
  height: 76px;
  border-bottom: 1px solid #e5e7eb;
  background: #ffffff;
}

.container {
  width: min(1180px, 92%);
  margin: 0 auto;
}

.navbar-content {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  text-decoration: none;
  color: #111827;
  font-size: 24px;
  font-weight: 700;
}

.nav-links {
  display: flex;
  gap: 32px;
}

.nav-links a {
  text-decoration: none;
  color: #4b5563;
  font-size: 15px;
}

.nav-links a:hover {
  color: #111827;
}

.nav-actions {
  display: flex;
  gap: 10px;
}

.login-button,
.signup-button {
  padding: 10px 18px;
  border-radius: 6px;
  cursor: pointer;
}

.login-button {
  border: 1px solid #d1d5db;
  background: #ffffff;
}

.signup-button {
  border: 1px solid #111827;
  background: #111827;
  color: #ffffff;
}
</style>