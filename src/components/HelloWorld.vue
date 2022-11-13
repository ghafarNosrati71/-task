<template>
  <div class="inputSherch">
    <input type="text" name="search" placeholder="Search.." />
    <select class="select" name="option">
      <option value="" disabled selected>Choose your option</option>
      <option value="1">Option 1</option>
      <option value="2">Option 2</option>
      <option value="3">Option 3</option>
    </select>
  </div>
  <section class="profile--container"
  @click="click">
    <article v-for="n in 8" :key="n" class="card">
      <img
      class="img"
        src="../assets/iran.png"
        alt="card image"
      />
      <article class="content">
        <h3>Iran</h3>
        <div>
          <p><b> population : </b>123.245.334.14</p>
          <p><b> Region : </b>Eruope</p>
          <p><b> Capital : </b>Berlin</p>
        </div>
      </article>
    </article>
    
  </section>
</template>

<script>
import "../assets/scss/album.css";
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data: function () {
    return {};
  },
  methods:{
    click(){
      this.$router.push("item")
    }
  }
};
</script>


