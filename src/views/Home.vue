<template>
  <div class="home">
    <h1>HomePage</h1>
    <p class="red white--text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui numquam omnis pariatur ducimus consequuntur quidem explicabo nam ullam minus ab asperiores porro illo eos, ipsum rem blanditiis ea sint aspernatur.</p>
    <p class="pink lighten-4 red--text text--darken-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus deserunt explicabo cumque repellat, excepturi architecto laboriosam nam repudiandae praesentium odit iste voluptatum accusamus. Rerum illum quaerat quas necessitatibus. Necessitatibus, ad.</p>
    <h1 class="display-4">Massive Display</h1>
    <h4 class="display-1">Smaller display</h4>
    <p class="headline">This is a headline</p>
    <p class="subheading">This is a subheading</p>
    <p class="caption">This is a caption</p>
    <v-btn class="pink white--text">click me</v-btn>
    <v-btn depressed color="pink" dark>click me</v-btn>
    <v-btn flat color="pink">click me</v-btn>

    <v-btn depressed class="pink white--text">
      <v-icon left>email</v-icon>
      <span>email me</span>
    </v-btn>

    <v-btn depressed small class="pink white--text">
      <v-icon left>email</v-icon>
      <span>email me</span>
    </v-btn>

    <v-btn depressed large class="pink white--text">
      <span>email me</span>
      <v-icon large right>email</v-icon>
    </v-btn>

     <v-btn fab depressed small dark color="purple">
      <v-icon>favorite</v-icon>
    </v-btn>
  </div>
</template>

<script>
  export default {
  
  }
</script>
