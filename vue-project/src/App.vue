
 <script>
 import Menu from './list.vue'
 export default {
 components: {
     Menu
 },
 data() {
     return{
         pageTitle: "My Vue",
         data: [
             {
                 id:1,
                 title: "Menu",
                 url: "https://www.youtube.com/"
             },
             {
                 id:2,
                 title: "Contact",
                 url: "https://www.youtube.com/"
             },
             {
                 id:3,
                 title: "About US",
                 url: "https://www.youtube.com/"
             },
         ]
     }
 }
 }
 
 </script>

 <template>
  <div class="div1">
    <ul>
       <li v-for="item in Link" :key="item.id">
      <a :href="item.url"> {{ item.name }}</a>
      </li>
    </ul>
  </div>

  <Menu :menuData="data"/>
 </template>
