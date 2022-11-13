<template>
  <div class="main" >
    <button class="back" @click="back">back</button>
  </div>
  <div class="item-show">
     <section >
   <img class="image" src="../assets/iran.png"/>
  </section>
  <section >
    <article class="card-item">
      <article class="content">
        <h3>Germany</h3>
        <div>
          <p><b> Native Name : </b>Iran</p>
          <p><b> population : </b>123.245.334.14</p>
          <p><b> Region : </b>Iran</p>
          <p><b> Capital : </b>Iran</p>
          <p><b> Sub Region : </b>Iran</p>
        </div>
        <div class="sub">
          <p><b> Border Countries : </b>Iran&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;iran &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iran</p>

        </div>
      </article>
    </article>
  </section>
  </div>
  
</template>
<script>

export default {
     methods:{
          back(){
               this.$router.push("/")

          }
     }
}
</script>

<style>
.main{
     width: 100%;
}
.back {
float: left;
  padding: 20px;
  color:gray;
  background-color: white;
  border-radius: 10px;
  border: 2px solid #d4d4d4;
  color: rgb(161, 159, 159);
  padding: 15px 32px;
  text-align: center;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
 
}
.item-show {
  margin-top: 3em;
  display: grid;
  grid-template-columns: repeat(2, 500px);
  grid-auto-rows: 50px;
  gap: 1rem;
}
.card-item{
     padding: 1px;
     margin-top: 2.5em;
     width: 450px;
     height: auto;
     border-radius: 10px;
  box-shadow: 2px 2px 2px -3px rgba(0, 0, 0, 0.2);
}
.image {
     padding: 1px;
     margin-top: 4em;
     width: 450px;
     height: 350px;
     border-radius: 10px;
  box-shadow: 2px 2px 2px -3px rgba(0, 0, 0, 0.2);
}
.sub{
     margin-top: 4em;
}
@media only screen and (max-width: 360px) {
  .item-show {
    margin-top: 3em;
    display: grid;
    grid-template-columns: repeat(1, 310px);
    grid-auto-rows: 220px;
    gap: 1rem;
  }
  .image {
    width: 320px;
    height: 200px;
    object-fit: cover;
    border-radius: 10px 10px 10px 10px;
  }
}
</style>