<template>
  <div class="container">
    <div class="date">{{data}}</div>

    <Shedule />

    <div class="buttons">
      <button v-on:click="logout">
        <img src="../../../public/img/student/btn1.svg" style="margin-top: 7px">
      </button>

      <button v-on:click="addLessons">
        <img src="../../../public/img/student/btn2.svg">
      </button>

      <button v-on:click="dialogue">
        <img src="../../../public/img/student/btn3.svg">
      </button>

      <button v-on:click="calendar">
        <img src="../../../public/img/student/btn4.svg">
      </button>
    </div>
  </div>
</template>

<script>
import Shedule from "@/components/stydent/Shedule";

export default {
  name: "MainScreen",

  components: {
    // Authorization,
    Shedule
  },

  data(){
    return{
      data: '25.05.2000'
    }
  },

  methods:{
    logout(){},
    addLessons(){},
    dialogue(){},
    calendar(){}
  }
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@300&display=swap');

  .container {
    padding-right: 5%;
    padding-left: 5%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100vh;
  }

  .date {
    border-radius: 15px;
    border: solid 1px transparent;
    border-color: #BDFFFFFF;
    background: #BDFFFFFF;
    height: 25px;
    width: 50%;
    text-align: center;
    font-size: 18px;
    margin-left: 25%;
    margin-top: 5%;
    font-family: 'Montserrat Alternates', serif;
  }

  .buttons {
    display: flex;
    justify-content: space-between;
    margin-bottom: 5%;
  }
  button {
    padding: 0;
    border: none;
    font: inherit;
    color: inherit;
    background-color: transparent;
    cursor: pointer;
  }
</style>