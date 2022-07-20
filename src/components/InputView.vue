<template>
 <div class="card" v-for="datas in data" :key="datas">
  <h3>{{datas.firstName}}{{datas.lastName}}</h3>
  <h3>{{datas.comment}}</h3>
 </div>
</template>

<script>
export default {
    props:{
        data:[],
        } 
}

</script>

<style>
input{
    margin-bottom: 5px;
}

</style>