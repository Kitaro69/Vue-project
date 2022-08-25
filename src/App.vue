<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <a href="/" ><img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /></a>

    <div class="wrapper">
      <HelloWorld msg="" />

      <nav>
         
         <RouterLink to="/personals">Data Personal</RouterLink>
         <RouterLink to="/skill">skills</RouterLink>
         
      </nav>
    </div>
  </header>

  <RouterView />
  <h2>Portofolio</h2>
  <div class="row row-cols-1 row-cols-md-2 g-4">
  <div class="col">
    <div class="card">
      <img src="src/assets/boostrap.jpg" class="card-img-top" alt="...">
      <div class="card-body bg-dark">
        <h5 class="card-title text-white">Bootstrap</h5>
       
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card">
      <img src="src/assets/1.jpg" class="card-img-top" alt="...">
      <div class="card-body bg-dark">
        <h5 class="card-title text-white">Mockup Aplikasi Peduli Diri</h5>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card">
      <img src="src/assets/2.jpg" class="card-img-top" alt="...">
      <div class="card-body bg-dark">
        <h5 class="card-title text-white">Indocement</h5>
      </div>
    </div>
  </div>
</div>

<footer class="bg-dark text-center text-white">
  <!-- Grid container -->
  <div class="container p-4 pb-0">
    <!-- Section: Social media -->
    <section class="mb-4">
      <!-- Facebook -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #3b5998;"
        href="#!"
        role="button"
        ><i class="fab fa-facebook-f"></i
      ></a>

      <!-- Twitter -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #55acee;"
        href="#!"
        role="button"
        ><i class="fab fa-twitter"></i
      ></a>

      <!-- Google -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #dd4b39;"
        href="#!"
        role="button"
        ><i class="fab fa-google"></i
      ></a>

      <!-- Instagram -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #ac2bac;"
        href="#!"
        role="button"
        ><i class="fab fa-instagram"></i
      ></a>

      <!-- Linkedin -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #0082ca;"
        href="#!"
        role="button"
        ><i class="fab fa-linkedin-in"></i
      ></a>
      <!-- Github -->
      <a
        class="btn btn-primary btn-floating m-1"
        style="background-color: #333333;"
        href="#!"
        role="button"
        ><i class="fab fa-github"></i
      ></a>
    </section>
    <!-- Section: Social media -->
  </div>
  <!-- Grid container -->

  <!-- Copyright -->
  <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
    © 2020 Copyright:
    <a class="text-white" href="https://mdbootstrap.com/">MDBootstrap.com</a>
  </div>
  <!-- Copyright -->
</footer>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
  margin-left: 450px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }

  .card{
    margin-top: 40px;
  }
   
   .container{
    margin-top: 100px;
   }
   .card-title{
    color: gray;
   }

   .card-text{
    color: gray;
   }

   h2{
    color: white;
   }
}
</style>
