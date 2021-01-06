<template>
<div>
    <hr>
    <p>auto populate filter</p>
    <input type="text" v-model="enteredText">
  
        <p v-for="city in enteredCityName" :key='city'> {{ city }} </p>
  
</div>
</template>

<script>
export default {
    data(){
        return{
            enteredText:'',
            cityNames:['Tenali','Vijayawada','Tirupati','Eluru','Bapatla','Vizag'],

        }
    },
    computed:{
        enteredCityName(){
           return this.cityNames.filter(data => {
                   return data.match(this.enteredText);
                }   
            );
        }
    }
}
</script>