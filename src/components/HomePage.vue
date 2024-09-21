<template>
  <v-container class="">
    <v-row class="main mx-auto mt-4">
      <v-col cols="12 pa-0 img">
        <img src="/src/assets/illustration-hero.svg" alt="" />
      </v-col>
      <v-col cols="12" class="summary d-flex justify-center align-center pt-5">
        Order Summary
      </v-col>

      <v-col
        cols="12"
        class="d-flex justify-center align-center py-0 px-15 para"
      >
        You can now listen to million of songs, audiobooks, and podcasts on any
        device anywhere you like!
      </v-col>

      <v-col cols="12" class="text-black py-3">
        <div class="mid d-flex align-center mx-5 px-2">
          <v-col cols="2" class="d-flex justify-center">
            <img class="img2" src="/src/assets/icon-music.svg" alt="" />
          </v-col>
          <v-col cols="6" class="d-flex flex-column text-left">
            <div class="text">Annual Plan</div>
            <div class="price">₹150/year</div>
          </v-col>
          <v-col class="change text-right">
            <a href="">Change</a>
          </v-col>
        </div>
      </v-col>

      <v-col class="d-flex justify-center align-center py-0 mx-5">
        <v-btn block class="btn1 text-capitalize" elevation="10"
          >Proceed to payment</v-btn
        >
      </v-col>

      <v-col class="d-flex justify-center align-center pb-5 mx-5">
        <v-btn block class="btn2 text-capitalize" flat>Cancel Order</v-btn>
      </v-col>
    </v-row>
  </v-container>
  <!-- <img src="/src/assets/pattern-background-desktop.svg" alt=""> -->
</template>

<script setup>
</script>

<style scoped>
@font-face {
  font-family: f1;
  src: url(/src/assets/RedHatDisplay-Black.ttf);
}
@font-face {
  font-family: f2;
  src: url(/src/assets/RedHatDisplay-Bold.ttf);
}
.main {
  background-color: #ffffff;
  width: 350px;
  height: 530px;
  border-radius: 10px;
}
.img img {
  width: 100%; /* Ensures the image fits within the width of the container */
  height: auto; /* Keeps the aspect ratio intact */
  display: block; /* Removes any spacing around the image */
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}
.mid {
  background-color: hsl(230, 75%, 98%);
  border-radius: 10px;
}
.text {
  font-family: f1;
  font-size: 12px;
}
.price {
  font-size: 12px;
  color: hsl(224, 23%, 55%);
}
.change {
  font-size: 11px;
  font-family: f2;
}
.change a {
  color: hsl(245, 75%, 52%);
  text-decoration: underline; /* Underline the link */
}

.change a:hover {
  text-decoration: none; /* Remove underline on hover */
  color: hsl(245, 83%, 68%);
}
.para {
  font-size: 12px;
  text-align: center;
  color: hsl(224, 23%, 55%);
}
.summary {
  font-family: f1;
  color: black;
  font-size: 18px;
}
.img2 {
  width: 130%;
}
.btn1 {
letter-spacing: .2px;  font-family: f2;
  background-color: hsl(245, 75%, 52%); /* Initial background color */
  color: white; /* Optional: Set text color to white for contrast */
}

.btn1:hover {
  background-color: hsl(245, 83%, 68%);
  color: white; /* Ensure text color remains readable */
}

.btn2 {
letter-spacing: .2px;  font-family: f2;
  background-color: white; /* Initial background color */
  color: hsl(224, 23%, 55%);
}

.btn2:hover {
  color: hsl(224, 26%, 25%); /* Ensure text color remains readable */
  background-color: #ffffff;
}
</style>