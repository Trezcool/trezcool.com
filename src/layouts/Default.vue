<template>
  <div class="layout">

    <header class="header">
      <g-link to="/">
        <div class="logo">
          <span class="logo__text">> $ cd /home/trezcool</span>
          <span class="logo__cursor"></span>
        </div>
      </g-link>

      <nav class="nav">
        <g-link class="nav__link" to="/about/">About</g-link>
        <g-link class="nav__link" to="/portfolio/">Portfolio</g-link>
        <g-link class="nav__link" to="/contact/">Contact</g-link>
        <g-link class="nav__link" to="/blog/">Blog</g-link>
      </nav>
    </header>

    <slot/>

  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
