<template>
  <div class="container">
    <div>
      <input v-model="login" placeholder="логин">
      <input type='password' v-model="password" placeholder="пароль">
      <button>войти</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Authorization",

  data(){
    return{
      login: '',
      password: ''
    }
  }
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@300&display=swap');

  .container{
    background: #DFFBFF;
    height: 100vh;
  }

  .container>div{
    margin-right: 5%;
    margin-left: 5%;
    padding-top: 30vh;
    display: flex;
    flex-direction: column;
  }

  input{
    border-radius: 15px;
    border-color: #55E5FA;
    height: 25px;
    margin-bottom: 3%;
    text-align: center;
    font-size: 20px;
    font-family: 'Montserrat Alternates',serif;
  }

  button{
    height: 35px;
    display: inline-block;
    text-align: center;
    text-decoration: none;
    margin-top: 10%;
    color: #252525;
    border: 1px solid #55E5FA;
    background-color: #55E5FA;
    border-radius: 15px;
    font-size: 20px;
    cursor: pointer;
    font-family: 'Montserrat Alternates',serif;
  }
  button:hover{
    background-color: white;
  }
</style>