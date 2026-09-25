<template>
  <div class="app">

    <!-- Navigation -->
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


    <!-- Hero -->
    <main>

      <section class="hero">
        <div class="container hero-content">

          <div class="hero-text">

            <p class="eyebrow">
              YOUR NEXT OPPORTUNITY STARTS HERE
            </p>

            <h1>
              Find work that moves
              <span>your life forward.</span>
            </h1>

            <p class="hero-description">
              Discover meaningful opportunities from companies
              looking for talented people like you.
            </p>

            <!-- Search -->
            <div class="search-box">

              <div class="search-field">
                <label>What are you looking for?</label>

                <input
                  type="text"
                  placeholder="Job title, skill or keyword"
                />
              </div>

              <div class="search-field">
                <label>Where?</label>

                <input
                  type="text"
                  placeholder="City or location"
                />
              </div>

              <button class="search-button">
                Search jobs
              </button>

            </div>

          </div>

        </div>
      </section>


      <!-- Featured Jobs -->
      <section class="featured-jobs">

        <div class="container">

          <div class="section-header">

            <div>
              <p class="section-label">
                OPPORTUNITIES
              </p>

              <h2>
                Featured jobs
              </h2>
            </div>

            <a href="#">
              View all jobs →
            </a>

          </div>


          <div class="job-grid">

            <article class="job-card">

              <div class="company-logo">
                A
              </div>

              <div class="job-content">

                <h3>
                  Frontend Developer
                </h3>

                <p class="company-name">
                  Acme Technologies
                </p>

                <p class="job-location">
                  Kigali · Full-time
                </p>

              </div>

              <button class="apply-button">
                Apply
              </button>

            </article>


            <article class="job-card">

              <div class="company-logo">
                B
              </div>

              <div class="job-content">

                <h3>
                  Backend Developer
                </h3>

                <p class="company-name">
                  Bright Systems
                </p>

                <p class="job-location">
                  Kigali · Full-time
                </p>

              </div>

              <button class="apply-button">
                Apply
              </button>

            </article>


            <article class="job-card">

              <div class="company-logo">
                C
              </div>

              <div class="job-content">

                <h3>
                  UI/UX Designer
                </h3>

                <p class="company-name">
                  Creative Labs
                </p>

                <p class="job-location">
                  Remote · Full-time
                </p>

              </div>

              <button class="apply-button">
                Apply
              </button>

            </article>

          </div>

        </div>

      </section>

    </main>

  </div>
</template>


<style>
/* =========================
   RESET
========================= */

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  color: #111827;
  background: #ffffff;
}

button,
input {
  font: inherit;
}


/* =========================
   GENERAL
========================= */

.container {
  width: min(1180px, 92%);
  margin: 0 auto;
}


/* =========================
   NAVBAR
========================= */

.navbar {
  height: 76px;
  border-bottom: 1px solid #e5e7eb;
  background: #ffffff;
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


/* =========================
   HERO
========================= */

.hero {
  padding: 100px 0 80px;
  background: #f8fafc;
}

.hero-content {
  text-align: center;
}

.eyebrow {
  margin-bottom: 18px;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 1.5px;
  color: #6b7280;
}

.hero h1 {
  max-width: 800px;
  margin: 0 auto;
  font-size: clamp(42px, 6vw, 68px);
  line-height: 1.05;
  letter-spacing: -2px;
}

.hero h1 span {
  display: block;
}

.hero-description {
  max-width: 650px;
  margin: 24px auto 0;
  color: #6b7280;
  font-size: 18px;
  line-height: 1.6;
}


/* =========================
   SEARCH
========================= */

.search-box {
  max-width: 900px;
  margin: 45px auto 0;
  padding: 10px;
  display: flex;
  gap: 10px;
  background: #ffffff;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
}

.search-field {
  flex: 1;
  text-align: left;
  padding: 8px 14px;
}

.search-field label {
  display: block;
  margin-bottom: 5px;
  font-size: 12px;
  font-weight: 600;
  color: #6b7280;
}

.search-field input {
  width: 100%;
  border: none;
  outline: none;
  color: #111827;
}

.search-button {
  padding: 0 28px;
  border: none;
  border-radius: 7px;
  background: #111827;
  color: #ffffff;
  cursor: pointer;
}


/* =========================
   FEATURED JOBS
========================= */

.featured-jobs {
  padding: 80px 0;
}

.section-header {
  display: flex;
  justify-content: space-between;
  align-items: end;
  margin-bottom: 30px;
}

.section-label {
  margin: 0 0 8px;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 1.3px;
  color: #6b7280;
}

.section-header h2 {
  margin: 0;
  font-size: 32px;
}

.section-header a {
  color: #111827;
  text-decoration: none;
  font-weight: 600;
}


/* =========================
   JOB CARDS
========================= */

.job-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
}

.job-card {
  padding: 24px;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  background: #ffffff;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.job-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.06);
}

.company-logo {
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  border-radius: 8px;
  background: #f3f4f6;
  font-weight: 700;
}

.job-content h3 {
  margin: 0 0 8px;
  font-size: 18px;
}

.company-name {
  margin: 0 0 6px;
  color: #374151;
}

.job-location {
  margin: 0;
  color: #6b7280;
  font-size: 14px;
}

.apply-button {
  width: 100%;
  margin-top: 22px;
  padding: 11px;
  border: 1px solid #d1d5db;
  border-radius: 6px;
  background: #ffffff;
  cursor: pointer;
}

.apply-button:hover {
  background: #f9fafb;
}


/* =========================
   MOBILE
========================= */

@media (max-width: 800px) {

  .nav-links {
    display: none;
  }

  .nav-actions {
    display: none;
  }

  .hero {
    padding: 70px 0 60px;
  }

  .search-box {
    flex-direction: column;
  }

  .search-button {
    padding: 14px;
  }

  .job-grid {
    grid-template-columns: 1fr;
  }

  .section-header {
    align-items: start;
    gap: 15px;
    flex-direction: column;
  }
}
</style>