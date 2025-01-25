<template>
  <nav class="navigation_tabs">
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active"><a class="nav-link" href="#home">Home <span class="sr-only">(current)</span></a></li>
      <li class="nav-item"><a class="nav-link" href="https://linktr.ee/leab_prazim" target="_blank">My LinkTree</a></li>
      <li class="nav-item"><a class="nav-link" href="#education">{{ tab_one }}</a></li>
      <li><a class="nav-link" href="#hobbies">{{ tab_two }}</a></li>        
      <li><a class="nav-link" href="#skills">{{ tab_three }}</a></li>
      <li><a class="nav-link" href="#certs">{{ tab_four }}</a></li>
    </ul>
  </div>
</nav> 



</template>

<script> 

export default {
  props: ['tab_one', 'tab_two', 'tab_three', 'tab_four'],
}
</script>

<style> 

ul>li{
  position: relative;
  list-style-type: none;
  display: inline-block;
  margin: 0 10px;
  
}

</style>