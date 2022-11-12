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
  <section class="profile--container">
    <article v-for="n in 8" :key="n" class="card">
      <img
        src="https://images.unsplash.com/photo-1612972412954-c7dd0e42ba4b?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=751&q=80"
        alt="card image"
      />
      <article class="content">
        <h3>Germany</h3>
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
};
</script>


