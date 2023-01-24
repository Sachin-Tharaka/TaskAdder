<template>
    <div class="container">
        
        <h2 class="header">User Profile</h2>
    
        <div class="form">
            <form action="">
                <input type="text" v-model="name" placeholder="Name">
                <button @click="submit">Submit</button>
            </form>
            <h5>{{ name }}</h5>
        </div>
    </div>

</template>

<script>
export default{
    data(){
        return{
            name: '',
        }
    },
    methods:{
        submit(){
            console.log(this.name);
        }
    }
}
</script>

<style scoped>
body{
    margin: 0;
    padding: 0px;
    box-sizing: border-box;
}
.container{
    margin: 0px auto;
    width: 600px;
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    background-color: rgb(201, 192, 192);
    
}

.form{
    display: flex;
    justify-content: center;
    background-color: rgba(199, 132, 65, 0.304);

}

.header{
}
</style>