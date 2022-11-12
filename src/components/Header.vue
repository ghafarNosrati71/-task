<template>
     <div class="header">
         <p class="p">Where is the world ?</p>
         <div class="theme-switch-wrapper">
       <label class="theme-switch" for="checkbox">
    <input type="checkbox" id="checkbox" @change="getData" v-model='sss' />
    <div class="slider round"></div>
  </label>
    <em>Enable Dark Mode!</em>
  </div>
     </div>
      
   </template>
   
   <script>
   import "../assets/scss/album.css";
   export default {
     // eslint-disable-next-line vue/multi-word-component-names
     name: "Header",
     props: {
       msg: String,
     },
     data: function () {
       return {
          sss:false
       };
     },
     methods:{
          getData(){
               var element = document.body;
                element.classList.toggle("dark-mode"); 
          }
     }
   };
   </script>
   <style scoped>
   .header{
     columns: 2;

   }
   .p{
     font-size: 1.5rem;
     font-weight: 900;
     
   }
   .button{
     padding: 20px;
     width: 100px;
     align-content: center;
     text-align: center;
     float: right;
     background-color: rebeccapurple;
   }
  
h1 {
    color: var(--heading-color);
    font-family: "Sansita One", serif;
    font-size: 2rem;
    margin-bottom: 1vh;
}

p {
  font-size: 1.1rem;
  line-height: 1.6rem;
}

a {
  color: var(--primary-color);
  text-decoration: none;
  border-bottom: 3px solid transparent;
  font-weight: bold;
  
}



.post-meta {
  font-size: 1rem;
  font-style: italic;
  display: block;
  margin-bottom: 4vh;
  color: var(--secondary-color);
}



/*slider switch css */
.theme-switch-wrapper {
  float: right;
  align-items: center;
  
}
em {
    margin-left: 10px;
    font-size: 1rem;
    text-align: center;
    align-content: center;
    align-items: center;
  }
.theme-switch {
  display: inline-block;
  height: 34px;
  position: relative;
  width: 60px;
}



.slider {
  background-color: #ccc;
  bottom: 0;
  cursor: pointer;
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
  transition: .4s;
}


.slider:before {
  background-color: rgb(0, 0, 0);
  bottom: 4px;
  content: "";
  height: 26px;
  left: 4px;
  position: absolute;
  transition: .4s;
  width: 26px;
}

input:checked + .slider::before {
  background-color: #ffffff;
}

input:checked + .slider:before {
  transform: translateX(26px);
}

.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
   </style>
   
   