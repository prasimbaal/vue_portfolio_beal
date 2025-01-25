<template> 
  <div class="main-container">
    <div class="navabr">
      <nav> <navbar tab_one="Education" tab_two="Hobbies" tab_three="Skills" tab_four="certifications" /> </nav>
    </div>
    <div class="flex-container">
      <div class="profile">
        <img src="./assets/beal.jpg" alt="">
        <div class="details">
          <h2>{{Full_N}}</h2>
          <h3>Software Engineer</h3>
          <h3> {{age}}</h3>
          <h3>{{ Location }} </h3>
        </div>
        <div class="services">
            <h3 v-for="Service in Services">{{Service}}</h3>
        </div>
        <div class="socials">
        <a href="https://t.me/bilboardmusic">telegram</a><br>
        <a href="https://github.com/prasimbaal">Github</a>
      </div>
      <div class="about">
          <about />
      </div>
    </div>
      </div>
  </div>

</template>

<script>
  import navbar from './components/navbar.vue'
  import about from './components/about.vue';
  import cards from './components/cards.vue';


  export default{
    socials: ['github','telegram','twitter', 'upwork'],
    skills: ['REST API', 'Django python', 'C++', 'vue.js', 'Cybersecurity'],
    
    components: {
      about,
      navbar
    },
    data(){
      return{
        Full_N: "Bealprasim Demere",
        age: 22,
        Location: "Hawassa, Ethiopia",
        Services: ['Web Development', 'Telegram-Bot Development']
      }
    }
  }

</script>

<style>

.profile{
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
} 

.details{
  flex: auto;
  margin-right: 20px;
}

.services{
  flex: auto;
}
.socials{
  flex: auto;
}

img{
  border-radius: 50%;
  height: 230px;
  width: 200px;
}

</style>