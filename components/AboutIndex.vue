<template>
  <v-container class="about section mt-10">
    <v-layout row wrap align-center>
      <v-flex xs12 sm6 px-3>
        <div class="about-thumb text-xs-center mb-4">
          <v-img
            src="https://cdn1.treatwell.net/images/view/v2.i1732194.w1080.h720.x07A6DC05/"
            aspect-ratio="1"
          ></v-img>
        </div>
      </v-flex>
      <v-flex xs-12 sm6 px-3>
        <div class="section-head">
          <h2 class="section-title">Presentation</h2>
          <div class="section-meta">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque
            voluptatibus iure, voluptates, saepe quos dolorum!
          </div>
        </div>

        <div class="section-body">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Similique
          aliquam, impedit. Blanditiis ab explicabo quidem saepe animi veniam,
          impedit ex sunt id quia vel totam?
        </div>
        <v-btn rounded color="#F48FB1" dark class="mt-4 mx-0" to="/about"
          >Lire la suite</v-btn
        >
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'AboutIndex',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about {
  position: relative;
  overflow: hidden;
}
</style>
