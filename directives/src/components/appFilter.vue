<template>
<div>
    <p v-text="haii_from_filter"></p>
    <input type="text" v-model="haii_from_filter">
    <p>{{ haii_from_filter | toUppercase}}</p>
    <p>{{ haii_from_filter | toUppercase}}</p>
</div>
</template>

<script>
export default {
    
    data(){
        return {
            haii_from_filter:'from app filter v-html directives'
        }
    },

    filters:{
        toUppercase(value){
            return value.toUpperCase();
        }
    }
}
</script>