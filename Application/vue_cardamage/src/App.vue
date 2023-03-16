<template>
  <div id="wrapper">
    <nav class="navbar  is-fixed-top is-spaced is-warning ">
      <div class="navbar-brand">
        <router-link to="/" class="navbar-item" > Fast Assurance</router-link>
          <!-- <img class="imgme1" src="@/assets/logo.png" alt="logo" > -->
      <a class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbar-menu" @click="showMobileMenu = !showMobileMenu">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
      </div>

      <div class="navbar-menu" id="navbar-menu" v-bind:class="{'is-active': showMobileMenu }">
       <div class="navbar-start">
          <!-- <div class="navbar-item">
            <form method="get" action="/search">
              <div class="field has-addons">
                <div class="control">
                  <input type="text" class="input" placeholder="What are you looking for?" name="query">
                </div>

                <div class="control">
                  <button class="button is-info">
                      <span class="icon">
                      <i class="fas fa-search"></i>
                      </span>
                  </button>
                </div>
              </div>
            </form>
          </div> -->
        </div>
        <div class="navbar-end">
          <router-link to="/login" class="navbar-item">Login</router-link>
          <router-link to="/detection-toolkit" class="navbar-item">Detection</router-link>
          <!-- <router-link to="/winter" class="navbar-item">Winter</router-link> -->
        
        <!-- <div class="navbar-item">
          <div class="buttons"> 
              <template v-if="$store.state.isAuthenticated">
                <router-link to="/my-account" class="button is-light">My account</router-link>
              </template>

              <template v-else>
                <router-link to="/log-in" class="button is-light">Log in</router-link>
              </template>
          </div>
        </div> -->
        </div>
      </div>
    </nav>

<!-- <div class="is-loading-bar has-text-centered" v-bind:class="{'is-loading': $store.state.isLoading }">
  <div class="lds-dual-ring"> </div>

</div> -->

  <section class="section">
    <router-view/>
  </section>

<div class="founders has-background-warning">

    <div class="columns">
      <div class="column">
        <!-- Add icon library -->
          <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

          <div class="card">
            <img src="@/assets/ligan.jpg" alt="Ben" class="imgme" >
            <h1>Bernardin LIGAN</h1>
            <p class="title-me">CEO & Founder</p>
            <p>UM6P University</p>
            <a href="#"><i class="fa fa-dribbble"></i></a>
            <a href="#"><i class="fa fa-twitter"></i></a>
            <a href="#"><i class="fa fa-linkedin"></i></a>
            <a href="#"><i class="fa fa-facebook"></i></a>
            <p><button  class="btme">Contact</button></p>
          </div>
      </div>

      <div class="column">
        <div class="card">
            <img src="@/assets/Aurel.jpg" alt="John" class="imgme" >
            <h1>Aurel TCHOKPONHOUE</h1>
            <p class="title-me">CEO & Founder</p>
            <p>UM6P University</p>
            <a href="#"><i class="fa fa-dribbble"></i></a>
            <a href="#"><i class="fa fa-twitter"></i></a>
            <a href="#"><i class="fa fa-linkedin"></i></a>
            <a href="#"><i class="fa fa-facebook"></i></a>
            <p><button  class="btme">Contact</button></p>
        </div>
      </div>

    </div>

    <div class="columns">

      <div class="column">
        <div class="card">
            <img src="@/assets/SANOGO.jpg" alt="John" class="imgme">
            <h1>Abroulaye SANOGO</h1>
            <p class="title-me">CEO & Founder</p>
            <p>UM6P University</p>
            <a href="#"><i class="fa fa-dribbble"></i></a>
            <a href="#"><i class="fa fa-twitter"></i></a>
            <a href="#"><i class="fa fa-linkedin"></i></a>
            <a href="#"><i class="fa fa-facebook"></i></a>
            <p><button  class="btme">Contact</button></p>
        </div>
        
      </div>

      <div class="column">
        <div class="card">
            <img class="imgme" src="@/assets/najoua.jpeg" alt="Najoua"  >
            <h1>Najoua OURTI</h1>
            <p class="title-me">CEO & Founder</p>
            <p>UM6P University</p>
            <a href="#"><i class="fa fa-dribbble"></i></a>
            <a href="#"><i class="fa fa-twitter"></i></a>
            <a href="#"><i class="fa fa-linkedin"></i></a>
            <a href="#"><i class="fa fa-facebook"></i></a>
            <p><button  class="btme">Contact</button></p>
      </div>
        
      </div>
    </div>
  </div>
  <footer class="footer">
    <p class="has-text-centered"> Copyright (c) 2022</p>
  </footer>

  </div>
</template>

<script>
import axios from 'axios'

export default {
  data(){
    return {
      showMobileMenu: false,
    }
  },
}

</script>





<style lang="scss">
@import "../node_modules/bulma";


.card {
  // box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  max-width: 300px;
  margin: auto;
  text-align: center;
}

.title-me {
  color: grey;
  font-size: 18px;
}

.btme {
  border: none;
  outline: 0;
  display: inline-block;
  padding: 8px;
  color: white;
  background-color: #000;
  text-align: center;
  cursor: pointer;
  width: 100%;
  font-size: 18px;
}

a {
  text-decoration: none;
  font-size: 22px;
  color: black;
}

.btme:hover, a:hover {
  opacity: 0.7;
}

.founders {
  margin-top: 10%;
  padding: 10%;
  background-color: yellow;
}

.imgme{
  width:80% ;
  height: 50%;
  /* border-radius: 50%;*/
  margin-top: 5%;
  border-color: white;
}

.imgme1{
  width: 100px;
  height: 100px;
  /* border-radius: 50%;*/
  padding-top: 2%;
  /* border-color: white;*/
}
</style>