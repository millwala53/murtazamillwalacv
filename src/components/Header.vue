<template>
    <v-toolbar flat color='secondary' class='py-2'>
      <v-toolbar-title dark class='white-color'>
        <h3>{{name}}</h3>
        <h5>{{designation}}</h5>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <a class='hidden-sm-and-down' href='https://github.com/millwala53' target="_blank" >
        <v-btn color='secondary' fab small  class='elavation-2'>
          <i class="fab fa-github headline  pointer"></i>
        </v-btn>
      </a>
      <a class='hidden-sm-and-down'>
        <v-btn color='secondary' fab small  class='elavation-2'>
          <i class="fab fa-linkedin headline  pointer"></i>
        </v-btn>
      </a>
      <a class='hidden-sm-and-down'>
        <v-btn color='secondary' fab small  class='elavation-2'>
          <i class="fab fa-facebook headline  pointer"></i>
        </v-btn>
      </a>
    </v-toolbar>
</template>

<script>
  export default{
    data(){
      return {
        name : "Murtaza Millwala",
        designation: "Software Engineer",
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang='scss'>
.white-color{
  color:white;
}
a{
  color: #3DADE5 !important;
}
</style>
