
<template>
  <div id="addi">
    <div id="ad1"><h1> Daily News</h1></div>
    <div id="ad2">
      <h2 v-for="d in articles">
       author : {{d.author}}<br>
       title : {{d.title}} 
       <hr>
      </h2>
    </div>
  </div>
</template>



<script>
  export default{
    name: 'App',
    data(){
      return{
        articles : [
          {
            author: "Livemint",
            title: "Long Covid More Severe In Women Than Men, Suggests Study - Mint",
          },
          {
            author: "Alex Reis",
            title: "Air pollution increases risk of getting COVID-19 in young adults - The European Scientist",
          },
          {
            author: "Prakash Nagarkatti and Mitzi Nagarkatti",
            title: "Why We Can't 'Boost' Our Way Out of the COVID-19 Pandemic in the Long Term – The Wire Science - The Wire Science",

          },
        ]

      }
    }
  }
</script>

<style>

h1{
  color: rgb(248, 248, 248);
}

#addi{
  background-color: rgb(197, 92, 127);
  display: flex;
}

#ad1{
  flex: 0.5;

}

#ad2{
  flex: 0.5;
  background-color: rgb(8, 3, 8);
}
</style>