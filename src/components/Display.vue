<template>

  <v-card class='elavation-2 pa-0'>
    <v-layout row wrap>
      <v-flex xs6 class='hidden-sm-and-down pr-0 py-0'>
        <v-card-media
          src= '/static/self.jpg'
          height="65vh"
          cover
        >
        </v-card-media>
      </v-flex>

      <v-flex xs12 sm12 md6 style='display:flex; flex-wrap:wrap; flex-direction: column;     justify-content: flex-end;' class='pl-0 py-0'>
        <v-card-title style='display: block;' class='mt-4' >
          <div style='width: fit-content;'>
            <p class='secondary white pa-1 caption ma-0 bubble'>HELLO & WELCOME</p>
            <div class='triangle'></div>
          </div>
          <h3 class='headline '>I'M <b class='text-lightblue'>MURTAZA MILLWALA</b></h3>
          <h5 class='body-2'> A Tech Geek With Ninja Coding Skills</h5>
        </v-card-title>
        <v-divider style='max-height:2px;'></v-divider>
        <v-card-text>
        <v-layout row wrap >

          <v-flex sm12 class='mt-2'>
            <v-layout row wrap>
              <v-flex xs3 ><b>Age</b></v-flex>
              <v-flex xs9 >26</v-flex>
            </v-layout>
          </v-flex>

          <v-flex sm12 class='mt-2'>
            <v-layout row wrap>
              <v-flex xs3 ><b>Address</b></v-flex>
              <v-flex xs9 >2A/1, 1st North St, Phase 1, DHA, Karachi, Pakistan</v-flex>
            </v-layout>
          </v-flex>

          <v-flex sm12 class='mt-2'>
            <v-layout row wrap>
              <v-flex xs3 ><b>Email</b></v-flex>
              <v-flex xs9 >millwala53@gmail.com</v-flex>
            </v-layout>
          </v-flex>

          <v-flex sm12 class='mt-2'>
            <v-layout row wrap>
              <v-flex xs3 ><b>Phone</b></v-flex>
              <v-flex xs9 >+92 332 3162348</v-flex>
            </v-layout>
          </v-flex>

          <v-flex sm12 class='mt-2'> 
            <v-layout row wrap>
              <v-flex xs3 ><b>Website</b></v-flex>
              <v-flex xs9 >milwala53.io</v-flex>
            </v-layout>
          </v-flex>
        </v-layout>
        </v-card-text>
        <v-card-actions style='width: 100%;' class='pa-0'>
          <v-flex class='secondary pa-1 ma-0'>
            <a class='secondary' href='https://github.com/millwala53' target="_blank" ><v-btn color='secondary' icon class='elavation-2'>
              <i class="fab fa-github headline  pointer"></i>
            </v-btn></a>
            <v-btn color='secondary' icon class='elavation-2'>
              <i class="fab fa-linkedin headline  pointer"></i>
            </v-btn>
            <v-btn color='secondary' icon class='elavation-2'>
              <i class="fab fa-facebook headline  pointer"></i>
            </v-btn>
          </v-flex>
        </v-card-actions>
      </v-flex>
    </v-layout>
  </v-card>

</template>

<script>
  export default{
    data(){
      return {
        name : "Murtaza Millwala",
        designation: "Software Engineer",
        show:true
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang='scss'>
.triangle {
  width: 0;
  border-top: 10px solid #3DADE5;
  border-left: 10px solid transparent;
  border-right: 10px solid transparent;
}
.bubble {
  width: fit-content;
  position: relative;
}
.white{
  color: white;
}
a{
  color: #3DADE5 !important;
}
</style>
