<template>
  <v-layout row wrap>
    <v-flex xs12 style='width:100%' class='pa-2 text-lightblue  headline text-sm-center' ><b>Projects</b></v-flex>
    <v-flex xs12>
      <v-layout row wrap >

        <v-flex xs12 sm12 md4 v-for='project in projects' :key='project.name' class='pointer' @click='openDialogue(project)'>
          <v-card class='py-3 white-color secondary project'  >
            <v-card-title >
              <b>{{project.name}}</b>
            </v-card-title>

          </v-card>
        </v-flex>

      </v-layout>
    </v-flex>



    <v-dialog v-model="dialog2" max-width="500px" >
        <v-card  style=' display:flex; flex-direction:column;'>
          <v-card-title>
           {{selected_project.name}}
          </v-card-title>
         <v-card-media v-bind:src="selected_project.image" height="250px"></v-card-media>
          <v-card-text>
            <v-layout row wrap>
              <v-flex>
                <p v-html='selected_project.description' ></p>
              </v-flex>
            </v-layout>
          </v-card-text>
          <v-card-actions>
            <v-btn color="primary" flat @click.stop="dialog2=false">Close</v-btn>
          </v-card-actions>
        </v-card>
    </v-dialog>
  </v-layout>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<script>
  export default{
    data(){
      return{
        dialog2: false,
        selected_project: {},
        projects:[
          {
            name: "Easy2Employ",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "Timezone App",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "xState",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "MoverMap",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "The Training Site",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "SpendTrac",
            description: "limitlo",
            image: "/static/e2e.png"
          },
          {
            name: "Qr Code Generator",
            description: "limitlo",
            image: "/static/e2e.png"
          }
        ]
      }
    },

    methods:{
      openDialogue(project){
        console.log('proje',project)
        this.selected_project = project
        this.dialog2 = true
      }
    }
  }


</script>

<style scoped>
.white-color{
  color:white;
}

.pointer{
  cursor: pointer;
}
.button-d{
    display: none;
  }
.project:hover{
  opacity: 0.4;
}
</style>
