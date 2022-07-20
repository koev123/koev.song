<template>
<div class="card">

    <form action="">
    <div class="form-group">
        <input type="text" placeholder="firstName" v-model="firstName">
    </div>
    <div class="form-group">
        <input type="text" placeholder="lastName" v-model="lastName">
    </div>
    <div class="form-group">
        <input type="text" placeholder="comment" v-model="comment">
    </div>
    <div class="form-group">
        <button @click="addForm">Add</button>
    </div>
  </form>
</div>
<Input :data="card"/>
</template>

<script>

 import Input from "./InputView.vue"
export default {
    components: {
        Input
    },
    data(){
        return{
            firstName:"",
            lastName:"",
            comment:"",
            card:[],
        }
    },
    methods:{
        addForm(event){
            event.preventDefault();
            let data = {};
            data.firstName=this.firstName;
            data.lastName=this.lastName;
            data.comment=this.comment;
            this.card.push(data);
            console.log(this.card);
            
        }
            
        }
  }



</script>

<style>
form{
    width: 90%;
    margin: auto;

}
Input{
    width: 90%;
    padding: 10px;
}
.card{
    box-shadow: rgba(0, 0, 0, 0.4) 0px 30px 90px;
    width: 50%;
    margin: auto;
    margin-top: 5px;
}
Button{
    padding: 10px;
    width: 95%;
    border: none;
    border-radius: 7px;
}

</style>