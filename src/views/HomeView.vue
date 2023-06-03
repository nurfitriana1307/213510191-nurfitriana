<template>
  <div class="home">
    <h1>Welcome to My App</h1>
    <p>My App is a web application that helps you manage your tasks and games.</p>
    <form @submit.prevent="addTask">
      <input type="text" v-model="newTask" placeholder="Enter task description">
      <button type="submit">Add Task</button>
    </form>
    <ul>
      <li v-for="(task, index) in tasks" :key="index">{{ task }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      tasks: [
        '',
        'My name is Nur Fitriana ',
        'You can call me Fitri'
      ],
      newTask: ''
    }
  },
  methods: {
    addTask() {
      if (this.newTask.trim() !== '') {
        this.tasks.push(this.newTask.trim())
        this.newTask = ''
      }
    }
  }
}
</script>

<style>
.home {
  padding: 1rem;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

li {
  margin-bottom: 0.5rem;
}
</style>
