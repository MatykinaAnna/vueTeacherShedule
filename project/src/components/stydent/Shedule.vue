<template>
  <div class="tableShedule" >

    <div>
      <div class="time">09:00</div>
      <div class="lesson">
        <div>
          {{arrayNameLessons[0]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">10:00</div>
      <div class="lesson" v-if="arrayLessons[1] == true">
        <div>
          {{arrayNameLessons[1]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">11:00</div>
      <div class="lesson" v-if="arrayLessons[2] == true">
        <div>
          {{arrayNameLessons[2]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">12:00</div>
      <div class="lesson" v-if="arrayLessons[3] == true">
        <div>
          {{arrayNameLessons[3]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">13:00</div>
      <div class="lesson" v-if="arrayLessons[4] == true">
        <div>
          {{arrayNameLessons[4]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">14:00</div>
      <div class="lesson" v-if="arrayLessons[5] == true">
        <div>
          {{arrayNameLessons[5]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">15:00</div>
      <div class="lesson" v-if="arrayLessons[6] == true">
        <div>
          {{arrayNameLessons[6]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">16:00</div>
      <div class="lesson" v-if="arrayLessons[7] == true">
        <div>
          {{arrayNameLessons[7]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">17:00</div>
      <div class="lesson" v-if="arrayLessons[8] == true">
        <div>
          {{arrayNameLessons[8]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">18:00</div>
      <div class="lesson" v-if="arrayLessons[9] == true">
        <div>
          {{arrayNameLessons[9]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">19:00</div>
      <div class="lesson" v-if="arrayLessons[10] == true">
        <div>
          {{arrayNameLessons[10]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>
    <div>
      <div class="time">20:00</div>
      <div class="lesson" v-if="arrayLessons[11] == true">
        <div>
          {{arrayNameLessons[11]}}
        </div>
        <button v-on:click="deleteLesson"><img src="../../../public/img/student/del.svg"></button>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "Shedule",

  methods: {
    deleteLesson(){

    }
  },

  data(){
    return{
      arrayLessons: [],
      arrayNameLessons: ['физика']
    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@300&display=swap');

  button {
    padding: 0;
    border: none;
    font: inherit;
    color: inherit;
    background-color: transparent;
    cursor: pointer;
  }

  .tableShedule>div{
    display: flex;
  }

  .time {
    font-family: 'Montserrat Alternates', serif;
    border-radius: 15px;
    border: solid 1px transparent;
    border-color: #55E5FA;
    background: #ffffff;
    height: 25px;
    width: 25%;
    font-size: 18px;
    margin-top: 15px;
    text-align: center;
  }

  .lesson {
    display: flex;
    width: 75%;
  }

  .lesson>div {
    border-radius: 15px;
    border: solid 1px transparent;
    border-color: #55E5FA;
    background: #55E5FA;
    height: 25px;
    text-align: center;
    margin-left: 15%;
    margin-top: 15px;
    width: 70%;
    font-family: 'Montserrat Alternates', serif;
  }

  .lesson>button {
    margin-top: 17px;
  }
</style>