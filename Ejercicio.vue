<template>

<div class="container-sm">
<h1 class="display-6">MOSTRAR DATOS</h1>
<table class="table table-success">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Titulo</th>
      <th scope="col">Body</th>
      <th scoper="col">Infor</th>
    </tr>
  </thead>
  <tbody v-for="(persona, index) in personas" :key="index">
    <tr>
      <th scope="row">{{persona.id}}</th>
      <td>{{persona.title}}</td>
      <td>{{persona.body}}</td>
      <router-link :to="`/usuario/${persona.id}`">Ver mas</router-link>
    </tr>
  </tbody>
</table>
</div>
</template>

<script>
export default {
    data(){
        return{
            personas:[],

        }
    },
    methods:{
         async getUser(){
             const data = await fetch('https://jsonplaceholder.typicode.com/posts');
             const info = await data.json();
             this.personas = info;
  
         }

    },
    created(){
     this.getUser();
     console.log(this.personas)
    }

}
</script>

<style>

</style>