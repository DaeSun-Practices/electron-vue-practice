<template>
  <v-container fluid>
    <v-card>
      <v-toolbar dense flat>
        <v-toolbar-title>문서편집기</v-toolbar-title>
        <v-spacer></v-spacer>   <!--이것은 우로 정렬을 의미한다.-->
        <v-btn setting>
          <v-icon>mdi-cog</v-icon>
        </v-btn>
      </v-toolbar>

      <v-card-text>
        <v-textarea v-model="text"></v-textarea>
      </v-card-text>

      <v-card-actions>
        <v-spacer></v-spacer> 
        <v-btn @click="read"> read </v-btn>
        <v-btn @click="write"> write </v-btn>
      </v-card-actions>


    </v-card>
  </v-container>
</template>

<script>


  export default{
    data(){
      return {
        text: '',
      }
    },

    methods: {
      read(){
        console.log("read")
      }

    }
  }
</script>
 