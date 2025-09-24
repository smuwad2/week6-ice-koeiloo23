<script>
    export default { 

       // add code here
       data(){
        return {
            loginOption:'username',
            username:'',
            emailOption:'email',
            email:''
        }
       }

    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
        
    <select v-model="loginOption">
        <option selected value="username">Username login</option>
        <option>Email login</option>
    </select>
    

    <div v-if="loginOption === 'username'">
        <label>Username</label>
        <input placeholder="Enter your username" >
       
    </div>

    <div v-else>
        <label>Email</label>
        <input placeholder="Enter your email" >
        
    </div>
</template>

