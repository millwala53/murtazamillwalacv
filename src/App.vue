<template>
  <v-app class='monteserrat app' >
      <Header />
      <v-container class='pt-3 grid-list-md' >
        <v-layout class=''>
          <v-flex class='m-auto pa-0' xs12 sm12 md9 lg8>
            <Display/>
          </v-flex>
        </v-layout>
        <v-layout class='my-5'>
          <v-flex class='m-auto' xs12 sm12 md9 lg8>
            <Skills/>
          </v-flex>
        </v-layout>
        <v-layout class='mb-5'>
          <v-flex class='m-auto' xs12 sm12 md9 lg8>
            <Projects/>
          </v-flex>
        </v-layout>
      </v-container>
  </v-app>
</template>

<script>
import Display from './components/Display'
import Header from './components/Header'
import Skills from './components/Skills'
import Projects from './components/Projects'

export default {
  data () {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [{
        icon: 'bubble_chart',
        title: 'Inspire'
      }],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  },
  name: 'App',
  components: {
    Display,
    Header,
    Skills,
    Projects
  }
}
</script>


<style lang='scss'>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');

.app{
  background-color: #e7e7e7 !important;
}

.bg-blue{
  background: url('/static/blue.png') !important;
      background-repeat: no-repeat;
    background-size: 300px 100px;
}


.monteserrat > *{
  font-family: 'Montserrat', sans-serif;
}

.m-auto{
  margin:auto;
}

.text-lightblue{
  color:#3DADE5;
}

</style>
