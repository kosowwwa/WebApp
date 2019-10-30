<template>
  <header class="header">
    <b-navbar class="p-0 fixed-bottom" toggleable="md" type="light">
        <div class="container">

      <b-navbar-nav>
        <li class="nav--link">
          <g-link to="/">
            <span class="oi oi-home"></span>
          </g-link>
        </li>
        <li class="nav--link">
          <g-link to="/about">
            <span class="oi oi-person"></span>
          </g-link>
        </li>
        <li class="nav--link">
          <g-link to="/blog">
            <span class="oi oi-briefcase"></span>
          </g-link>
        </li>
        <li class="nav--link">
          <g-link to="/contact">
            <span class="oi oi-envelope-closed"></span>
          </g-link>
        </li>
      </b-navbar-nav>

      </div> <!-- Container -->
    </b-navbar>
  </header>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang="scss">
nav {
  width: 100%;
  padding: 1rem !important;
  background: #000;
  ul {
    flex-direction: inherit !important;
    justify-content: space-around;
    width: 100%;
  }
  .nav--link {
    display: inline;
  }
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.logo-home {
  font-size: 24px;
  max-width: 75%;
  font-weight: bold;
  margin-left: 1rem;
  &:hover {
    text-decoration: none;
  }
}

.logo-desktop {
  @media(max-width: 419px) {
    display: none;
  }
  @media (min-width: 420px) {
    display: default;
  }
}

.logo–mobile {
  @media(max-width: 419px) {
    display: default;
  }
  @media (min-width: 420px) {
    display: none;
  }
}

.logo-image {
  width: 120px;
}

.nav--link {
  margin-left: 20px;
  @media (max-width: 419px) {
    margin: 0;
    padding: 15px 10px 10px 0;
  }
}

.active--exact {
  font-weight: bold;
  color: #d1a74f;
}
</style>
