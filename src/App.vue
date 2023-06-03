<template>
  <header>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      <router-link to="/myapp">My App</router-link>
    </nav>
  </header>
  <main>
    <router-view></router-view>
  </main>
  <footer>
    <p>&copy; 2023_Nur Fitriana_My App</p>
  </footer>
</template>

<script>
export default {
  name: 'App'
}
</script>


     <!--Nouse event-->
     <div class="box"></div>
     <div class="box"></div>
     <div class="box"></div>
     <div class="box"></div>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #06b66c;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.app {
display: flex;
flex-direction: column;
min-height: 100vh;
}

header {
background-color: #173826;
color: white;
padding: 1rem;
}

nav {
display: flex;
justify-content: flex-end;
align-items: center;
}

nav a {
color: white;
margin-left: 1rem;
}
    
main {
flex-grow: 1;
padding: 1rem;
}
    
footer {
background-color: #173826;
color: white;
padding: 1rem;
text-align: center;
}    
</style>
