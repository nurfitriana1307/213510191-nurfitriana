<template>
    <div class="myapp">
      <h1>Welcome to My App</h1>
      <p>My App is a web application that helps you manage your tasks.</p>
      <form @submit.prevent="addTask">
        <input type="text" v-model="newTask" placeholder="Enter task description">
        <button type="submit">Add Task</button>
      </form>
      <ul>
        <li v-for="(task, index) in tasks" :key="index">{{ task }}</li>
      </ul>
     <P>Setelah mengklik Game Catur, harap di refresh agar dapat memainkan game catur online.</P>
      <router-link to="catur.html" class="button">Game catur</router-link>
    </div>
  </template> 

<script>
export default {
  name: 'myapp'
}
</script>

<style>
.myapp {
  padding: 1rem;
}
.myapp{
  padding: 1rem;
}

.button {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  background-color: #007bff;
  color: #fff;
  border-radius: 0.25rem;
  text-decoration: none;
}

.button:hover {
  background-color: #0069d9;
}
</style>
