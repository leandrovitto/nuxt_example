<template>
  <div class="h-screen w-full p-10 bg-gray-100 text-3xl mx-auto">
  <!--  <pre><code>{{posts}}</code></pre> -->
  <div class="grid grid-cols-3 gap-4">
    <Card v-for="post in posts" :key="post.id" 
          :title="post.title" 
          :createDate="post.createdDate"
    />
  </div>

  </div>
</template>

<script>
export default {
  data(){
    return {
      posts : [
        { id : 1,title : "Titolo 1 Semidinamico" , createdDate : "13 min ago"},
        { id : 2,title : "Titolo 2 Semidinamico" , createdDate : "43 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
        { id : 3,title : "Titolo 3 Semidinamico" , createdDate : "23 min ago"},
      ]
    }
  },
  
}
</script>


<style>
    .hide-scroll-bar {
  -ms-overflow-style: none;
  scrollbar-width: none;
}
.hide-scroll-bar::-webkit-scrollbar {
  display: none;
}
</style>
