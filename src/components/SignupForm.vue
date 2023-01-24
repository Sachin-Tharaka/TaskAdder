<template>
    <form @submit="handleSubmit">
        <label for="">Email:</label>
        <input type="email" required>

        <label for="">Password:</label>
        <input type="password" required>
        
        <div class="submit">
            <button>Create an account</button>
        </div>
    </form>  
    
</template>

<style scoped>
body{
    display: flex;
    flex-direction: column;
    max-width: 420px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #fff;
    text-align: left;
 
}

label {
    margin: 25px 0 15px;
}
 
input {
    padding: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
    border: none;
    border-bottom: 1px solid #ddd;
}

.submit{
    padding: 0px auto;
    text-align: center;
}

button {
    padding: 10px 20px;
    border-radius: 20px;
    margin-top:20px;
    border: none;
}

</style>