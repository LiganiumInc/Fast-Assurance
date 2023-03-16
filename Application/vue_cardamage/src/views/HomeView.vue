<template>

  <div class="bg-img">
    <!-- <section class=" bg-img ">  -->
      <div class="hero-body has-text-centered "> 
          <p class="title is-1 mn-6 has-text-warning">
            Welcome to Smart Detection 
          </p>
          <p class="subtitle is-3 has-text-white">
              The best Car Damage Detection Portal online.
              <!-- Note: The batch_sizes given are samples used for google colab. If you are using a less powerful GPU, reduce your batch size, for example a PC with a 4G RAM GPU you should use a batch size of 1 for both resnet50 or resnet101. I used a batch size of 1 to train my model on my PC’s GPU, train for less than 100 epochs and it produced a validation loss of 0.263. This is favourable because my dataset is not large. A PC with a more powerful GPU you can use a batch size of 2. If you have a large dataset with more classes and much more images use google colab where you have free access to a single 12GB NVIDIA Tesla K80 GPU that can be used up to 12 hours continuously. Most importantly try and use a more powerful GPU and train for more epochs to produce a custom model that will perform efficiently across multiple classes. Achieve better results by training with much more images. 300 images for each each class is recommended to be the minimum required for training. -->
          </p>
         </div>
    <!-- </section>  -->
  </div> 


  <!-- <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div> -->
</template>

<script>

</script>

<style>
.bg-img { 
        background-image: url(../assets/baground1.webp) ;
        background-position: center center;
        background-repeat:  no-repeat;
        /* background-attachment: ; */
        background-size:  cover;
        /* background-color: #999; */

        margin-top: 0%;
        margin-left: 0%;
        margin-right: 0%;
        padding-top: 20%;
        padding-bottom: 30%;

 }

 p {
  color:darkred;
 }
</style>
