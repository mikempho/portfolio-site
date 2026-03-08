<template>
  <div class="page">
    <!-- Links -->
    <nav>
      <NuxtLink to="/">Home</NuxtLink>
      <NuxtLink to="/projects">Projects</NuxtLink>
      <NuxtLink to="/contact">Contact</NuxtLink>
    </nav>
    
    <NuxtPage/>
  </div>
</template>

<script setup>

</script>

<style>
  nav {
    text-align:center;
    padding:30px;
  }

  nav a {
    color:#000000;
    background-color:aliceblue;
    padding:10px;
    margin: 0px 40px;
    text-decoration:none;
    border-radius: 20px;
  }

  body {
    font-family: Verdana, Tahoma, sans-serif;
    background-color:#000000;
    color:aliceblue;
    width:75%;
    margin:auto;
  }

  nav a:hover {
    background-color:#d1ab4c;
  }
</style>