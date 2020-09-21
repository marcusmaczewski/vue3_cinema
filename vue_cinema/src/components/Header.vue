<template>
  <nav>
    <div class="logo">
      <img alt="Vue logo" src="../assets/logo.png">
    </div>
    <div class="menu">
      
      <div id="nav">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/user/">User</router-link>
      </div>
      <router-view/>
      
    </div>
  </nav>
</template>

<script>



export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  nav{
    background-color: #1d2633;
    padding: 25px 20px;

    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  nav .logo img{
    width: 30px;
  }

  ul{
    padding: 0;
    margin: 0;
  }

  li{
    list-style-type: none;
    display: inline-block;
  }

  li:not(:last-child){
    margin-right: 20px;
  }

  a{
    color: white;
    text-decoration: none;
  }


</style>
