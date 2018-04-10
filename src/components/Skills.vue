<template>
  <v-layout row wrap>
    <v-flex xs12 style='width:100%' class='pa-2 text-lightblue  headline text-sm-center' ><b>Skills</b></v-flex>
    <v-card class='pa-2 elavation-2' style='width:100%'>
      <v-layout row wrap>
        <v-flex class='px-2' xs6 v-for='skill in skills' :key='skill.name'>
            <b>{{skill.name}}</b>
            <v-progress-linear height="2" color='secondary'  v-model="skill.value"></v-progress-linear>
            <p class='caption' >{{skill.list}}</p>
        </v-flex>
      </v-layout>
    </v-card>
  </v-layout>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<script>
  export default{
    data(){
      return{

        skills:[
          {name: "Javascript", value:100, list: "VueJS, Angular4, Ionic, NativeScript"},
          {name: "PHP", value:100, list: "Custom PHP, Laravel, Lumen"},
          {name: "Databases", value:100, list: "MongoDb, MYSQL, PostgreSQL"},
          {name: "Tools", value:100, list: "NPM, GIT, Heroku, Yarn"},
        ]

      }
    }
  }


</script>

<style scoped>

</style>
