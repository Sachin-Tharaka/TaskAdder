<template>
    <div class="container">
        <h2 class="header2">Vue Task Changer</h2>
        <div class="content">
            <input type="text" v-model="input">
            <button @click="addGoal">Add a Goal</button>
        </div>
        <p v-if="goals.length === 0">No goals added here.Please add some</p>
        <div class="goalArea">
            <h2>My goals</h2>
            <ul class="goalscontainer" >
                <li class="qw" v-for="goal in goals" :key="goal" @click="deleteGoal">{{goal}}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  data(){
    return {
        input: '',
        goals: []
    }
  },
  methods:{
    addGoal(){
        this.goals.push(this.input)
        this.input = ''
    },
    deleteGoal(){
        this.goals.splice(this.goals.indexOf(this.input), 2)
    }
  }
}
</script>

<style>
.container{
  width: 400px;
  height:600px;
  display: flex;
  padding: 30px;
  margin: 0 auto;
  justify-content: center;
  flex-direction: column;
  background-color: rgb(39, 37, 37);
  border-radius: 10px;
  color: bisque;
}

.header2{
    background-color: rgb(68, 66, 66);
    text-align: center;
    padding:20px;
    border-radius: 10px;
}

.content {
    background: rgb(93, 92, 92);
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    padding: 30px;

}

.goalscontainer{
    margin: 20px auto;
    background: rgb(93, 92, 92);
    border-radius: 10px;
    display: flex;
    padding: 20px;
    width: 200px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    list-style-type: none;

}
.qw{
    background-color: rgb(127, 122, 122);
    padding: 5px 10px;
    border-radius: 20px;
    margin-bottom: 10px;
    cursor: pointer;
}
</style>