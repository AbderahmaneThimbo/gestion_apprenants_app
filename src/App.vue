<template>
  <header>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container">
        <RouterLink class="nav-link" to="/">
          <img src="./assets/logo.jpg" alt="Logo de l'application" />
        </RouterLink>

        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">

            <li class="nav-item me-3">
              <RouterLink class="nav-link" to="/apprenants">
                <i class="fas fa-users me-2"></i> Gestion des apprenants
              </RouterLink>
            </li>

            <li class="nav-item me-3">
              <RouterLink class="nav-link" to="/modules">
                <i class="fas fa-cogs me-2"></i> Gestion des modules
              </RouterLink>
            </li>

            <li class="nav-item me-3">
              <RouterLink class="nav-link" to="/inscription">
                <i class="fas fa-edit me-2"></i> Gestion des inscriptions
              </RouterLink>
            </li>

            <li class="nav-item me-3">
              <RouterLink class="nav-link" to="/payment">
                <i class="fas fa-credit-card me-2"></i> Gestion des paiements
              </RouterLink>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>

  <div class="container contenu">
    <RouterView />
  </div>
</template>

<style scoped>
img {
  width: 70px;
}


.navbar-nav .nav-link {
  font-size: 14px;
  font-weight: 500;
  color: #333;
  display: flex;
  align-items: center;
  transition: color 0.3s ease;
}


.navbar-nav .nav-link:hover {
  color: #1abc9c;
}

.navbar-nav .nav-link i {
  font-size: 18px;
}


.navbar-nav .nav-item {
  margin-right: 20px;
}
</style>
