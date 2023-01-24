<template>
 <div class="div1">
   <ul>
    <li v-for="item in list" :key="item.index">{{ item }}</li>
   </ul>
 </div>

</template>

<script>
export default{
    data(){
        return{
            list: ["Home","Product","Contact","AboutUs"]
        }
    }
}

</script>

<style>
ul {
    display: flex ;
    margin-left: 350px
} 

li {
    color: rgba(151, 33, 236, 0.874);
    width: 95px;
    font-weight: 600;
}
    
</style>