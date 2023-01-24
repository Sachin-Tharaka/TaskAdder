<template>
<!-- <UserProfile/> -->
<!-- <SignupForm/> -->
<TaskAdder/>
  
</template>


<script>
//import SignupForm from './components/SignupForm.vue';
//import UserProfile from './components/UserProfile.vue';
import TaskAdder from './components/TaskAdder.vue';


export default {
  name: 'App',
  components: {
    TaskAdder
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body{
  background-color: #eee;
  margin: 0;
}
</style>
