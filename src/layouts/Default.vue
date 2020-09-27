<template>
  <div class="custom">
    <div class="custom-shape-divider-top-1601172894">
      <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z" class="shape-fill"></path>
      </svg>
    </div>

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

      <footer>
        <p class="footer__copyright">© 2020 • Trésor Kambembo</p>
      </footer>
    </div>

    <div class="custom-shape-divider-bottom-1601175391">
      <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
<!--        <path d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z" class="shape-fill"></path>-->
<!--        <path d="M649.97 0L599.91 54.12 550.03 0 0 0 0 120 1200 120 1200 0 649.97 0z" class="shape-fill"></path>-->
        <path d="M600,16.8c0-8.11-8.88-13.2-19.92-13.2H0V120H1200V3.6H619.92C608.88,3.6,600,8.66,600,16.8Z" class="shape-fill"></path>
      </svg>
    </div>
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
.custom {
  position: relative;
  /*z-index: -10;*/
}
/** ---------- Header Divider ---------- **/ /* TODO: animate */
.custom-shape-divider-top-1601172894 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
  z-index: -1;
}
.custom-shape-divider-top-1601172894 svg {
  position: relative;
  display: block;
  width: calc(127% + 1.3px);
  height: 13rem;
}
.custom-shape-divider-top-1601172894 .shape-fill {
  fill: #181F24;
  /*fill: #1F282E;*/
  /*fill: #1E272E;*/
  /*animation: svganim 50s infinite forwards;*/
}
@media (max-width: 767px) {  /** For mobile devices **/
  .custom-shape-divider-top-1601172894 svg {
    width: calc(127% + 1.3px);
    height: 10.6rem;
  }
}
@keyframes svganim {
  0% { d: path("M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z"); }
  50% { d: path("M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z"); }
  100% { d: path("M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z"); }
}

/** ---------- Footer Divider ---------- **/ /* TODO: animate */
.custom-shape-divider-bottom-1601175391 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  z-index: -1;
}
.custom-shape-divider-bottom-1601175391 svg {
  position: relative;
  display: block;
  width: calc(127% + 1.3px);
  height: 7rem;
}
.custom-shape-divider-bottom-1601175391 .shape-fill {
  fill: #181F24;
}
@media (max-width: 767px) {  /** For mobile devices **/
  .custom-shape-divider-bottom-1601175391 svg {
    width: calc(127% + 1.3px);
    height: 6.2rem;
  }
}


/* ------- Base ------- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font: 62.5% Georgia, serif;  /* 10px (default) */
}

body {
  /* TODO: self-host Google's "Alegreya" font */
  font-family: Alegreya, -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  font-size: 1.8rem;
  background-color: #1E272E;
  /*background-color: #0A1E29;*/
  /*background-color: #091B25;*/
  /*background-image: linear-gradient(to right, #1E272E 0%, #33424D 100%);*/
  color: #D1C1A8;
  line-height: 1.5;
  min-height: 100%;
}

img {
  display: block;
  max-width: 100%;
}

.layout {
  height: 100vh;
  max-width: 76rem;
  margin: 0 auto;
  padding-left: 2rem;
  padding-right: 2rem;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2rem;
  height: 8rem;
}

.nav__link {
  margin-left: 2rem;
}
.nav__link, a {
  color: #D1C1A8;
  text-decoration: none;
}

/* ------- Logo ------- */
.logo {
  font-family: "Gill Sans", sans-serif;
}
.logo__text {
}
.logo__cursor {
  display: inline-block;
  width: 0.8rem;
  height: 1.25rem;
  background: #fe5186;
  margin-left: 0.5rem;
  border-radius: 0.1rem;
  animation: cursor 1s infinite;
}
@keyframes cursor {
  0% { opacity: 0; }
  50% { opacity: 1; }
  100% { opacity: 0; }
}

footer {
  position: fixed;
  height: 5rem;
  width: 76rem;
  bottom: 0;
  margin-bottom: 0;

  display: flex;
  justify-content: center;
  align-items: center;
}
.footer__copyright {
  font-size: 1.4rem;
}
</style>
