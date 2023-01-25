
      <script>
      export default {
    props: {
        menuData : {type : Array , required:true}
    
    },
    data(){
        return{

        }
    }
       }
      </script>

      <template>
        <ul>
    <li v-for="item in menuData" :key="item.id">
     <a :href="item.url">{{ item.title }}</a>
     </li>
    </ul>
      </template>