<template>
  <nav class="d-flex nav-holder">
    <h1>SHOP</h1>
    <ul class="d-flex nav-items">
      <li><router-link to="/" class="nav-link">Home</router-link></li>
      <li><router-link to="/products" class="nav-link">Products</router-link></li>
      <li><router-link to="/about" class="nav-link">About</router-link></li>
    </ul>
  </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
  h1{
    margin: 0;
  }

  nav {
    align-items: center;
    padding: 0 2rem;
    background-color: darkslategray;
    color: #fff;
  }
  .nav-items{
    margin-bottom: 10px;
    margin-top: 10px;
    margin-left: 40px;

  }

  li {
    list-style: none;
  }
  .nav-link {
    text-decoration: none;
    color: #fff;
    padding: 1rem;
    margin-right: 1.5rem;
    display: inline-block;
  }
  .nav-link:hover {
    background-color: #00000031;
    cursor: pointer;
  }
  .router-link-exact-active {
    text-decoration: underline;
  }
</style>