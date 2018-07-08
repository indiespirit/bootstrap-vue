<template>
  <b-navbar
    toggleable="md"
    class="navbar-dark bd-navbar"
    sticky>

    <b-navbar-toggle target="bd-main-nav"/>

    <b-navbar-brand
      to="/"
      exact>
      <svg
        class="d-block"
        width="36"
        height="36"
        viewBox="0 0 612 612"
        xmlns="http://www.w3.org/2000/svg"
        focusable="false"
        fill="#fff">
        <path
          d="M510,8 C561.846401,8.16468012 603.83532,50.1535995 604,102 L604,510 C603.83532,561.846401 561.846401,603.83532 510,604 L102,604 C50.1535995,603.83532 8.16468012,561.846401 8,510 L8,102 C8.16468012,50.1535995 50.1535995,8.16468012 102,8 L510,8 L510,8 Z M510,0 L102,0 C45.9,6.21724894e-15 0,45.9 0,102 L0,510 C0,566.1 45.9,612 102,612 L510,612 C566.1,612 612,566.1 612,510 L612,102 C612,45.9 566.1,6.21724894e-15 510,0 Z"
          fill-rule="nonzero"/>
        <text
          id="BV"
          font-family="Arial"
          font-size="350"
          font-weight="light"
          letter-spacing="2">
          <tspan
            x="72.0527344"
            y="446">B</tspan>
          <tspan
            x="307.5"
            y="446">V</tspan>
        </text>
      </svg>
      <span class="sr-only">Home</span>
    </b-navbar-brand>

    <b-collapse
      is-nav
      class="justify-content-between"
      id="bd-main-nav">

      <b-navbar-nav>
        <b-nav-item
          to="/docs"
          exact>Docs</b-nav-item>
        <b-nav-item to="/docs/components">Components</b-nav-item>
        <b-nav-item to="/docs/directives">Directives</b-nav-item>
        <b-nav-item to="/docs/reference">Reference</b-nav-item>
        <b-nav-item to="/docs/misc">Misc</b-nav-item>
        <b-nav-item to="/play">Play</b-nav-item>
      </b-navbar-nav>

      <b-navbar-nav>


      </b-navbar-nav>

    </b-collapse>
  </b-navbar>
</template>

<style>
.main-nav {
  box-shadow: 0 0 5px rgba(57, 70, 78, 0.2) !important;
  background: white;
  z-index: 1050;
  padding-bottom: 0;
}

.main-nav .nav-link,
.main-nav .navbar-brand {
  padding-bottom: 10px;
  border-bottom: 3px solid transparent;
}

.main-nav .nav-link.nuxt-link-active {
  border-bottom: 3px solid #4fc08d;
}

.navbar-brand img {
  height: 1.5em;
  padding-right: 0.5em;
}
</style>

<script>
import { version } from '~/content'

export default {
  computed: {
    version: () => version
  }
}
</script>
