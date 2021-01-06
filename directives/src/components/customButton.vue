<template>
  <div >
    <p>onclick custom</p>
    
    <button v-customClick="clicked"> click here for custom button </button>
  </div>
</template>

<script>
export default {
  name: 'customButton',



  directives:{
    customClick:{
      bind(el,binding){
        el.onclick = function(){
          binding.value();
        }
      }
    }
  },
  methods:{
    clicked(){
      alert(' hai i am from custom event')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
