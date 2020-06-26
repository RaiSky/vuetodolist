<template>
  <div id="app">
    <taskList :tasks="tasks"></taskList>
  </div>
</template>

<script>
import  taskList from './components/task-list';
export default {
  name: 'App',
  components: {
    taskList,
  },
  data(){
    return {
    tasks: [
      {
        title: 'Learn Basic Vuejs',
        completed: true
      },
      {
        title: 'Create todo app on Vuejs',
        completed: true
      },
      {
        title: 'Create shop on Vuejs',
        completed: false
      }
    ]
    }
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: right;
  margin-top: 60px;
}
</style>
