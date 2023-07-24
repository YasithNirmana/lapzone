<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>     
  <div class="body">
      <div class="header_top_bar">
        <div class="htb_contact_info">
          <span>info@lapzone.com</span>
          <span>|</span>
          <span>+1 234 567 8923</span>
        </div>
        <div class="htb_menu">
          <span>Home</span>
          <span>|</span>
          <span>About Us</span>
          <span>|</span>
          <span>Contact Us</span>
        </div>
      </div>
      <div class="header_main_bar">
        <span class="hmb_logo">LAPZONE</span>
          <div class="hmb_content">
            <span class="hmb_categories_menu">Categories <span class="material-symbols-outlined">expand_more</span></span>
            <div class="hmb_search">
              <input type="text"/>
              <span>|</span>
              <select>
                <option>All Categories</option>
              </select>
            </div>
            <span class="material-symbols-outlined">person</span>
            <span class="material-symbols-outlined">shopping_cart</span>
        </div>
      </div>
        
        <!-- <HelloWorld msg="You did it!" /> -->

        <!-- <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </nav> -->
      

    <!-- <RouterView /> -->
  </div>
  </template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Braah+One&display=swap');
.body{
  background-color: white;
}
.header_top_bar, .header_main_bar{
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 2px solid black;
  padding: 5 5px;
}
.htb_contact_info, .htb_menu{
  display: flex;
}
.htb_contact_info span, .htb_menu span{
  margin-left: 10px;
  margin-right: 10px;
}
.hmb_logo{
  font-size: 48px;
  font-family: 'Braah One', sans-serif;
  margin-left: 10px;
}
.hmb_content{
  width: 100%;
  display: flex;
  margin-left: 20px;
}
</style>
