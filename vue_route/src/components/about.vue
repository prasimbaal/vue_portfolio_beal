<template> 
    <div class="about">
        <div id="stack" v-for="stack in stacks">
            {{ stack }}
        </div>
        <div id="projects" v-for="project in projects">
            <a> {{ project }} </a>            
        </div>
    </div>
</template>

<script> 

export default{
    stacks: ['Django RESTAPI and Mysql', 'Python-Telegram Bot', 'Vue.js'],
    projects: ['Suq bot Telegram wit PTB', 'This portfolio website with vue.js', 'Skill-hub E-learning platform with Django and RESTAPI'],
    hobbies: ['Gaming', 'Coding', 'CTFs', 'Music',],
    certs: [],
}

</script>

<style scoped>
.about{
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
}

.projects{
    flex:auto;
    margin-right: 10px;
}

</style>