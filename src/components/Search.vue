<template>
  <div class="search">
    <input type="text" placeholder="键入内容！EX" />
    <div class="hotWord">
      <ul class="list">
        <li><a href="">工具</a></li>
        <li><a href="">工具</a></li>
        <li><a href="">工具</a></li>
        <li><a href="">工具</a></li>
      </ul>
      <div class="clear"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Search",
};
</script>

<style scoped>
@import "../assets/css/input.css";

a {
  display: inline-block;
  text-decoration: none;
  width: 50px;
  color: var(--bg-color);
  line-height: 20px;
  border-radius: 5px;
  transition: all 0.2s ease-out;
}

a:hover {
  background-color: rgba(29, 29, 29, 0.2);
}

.search {
  margin: 15px auto;
  height: 150px;
  min-width: 80%;
  max-width: 80%;
}
input {
  margin-top: 45px;
  /* font-size: 18px !important; */
  /* font-weight: bold; */
  width: 350px;
  height: 40px;
  color: var(--bg-color);
  font-size: 16px;
}

input::-webkit-input-placeholder {
  color: var(--bg-color);
}

input:focus {
    border: 2px solid var(--bg-color);
    background-color: rgba(29, 29, 29, 0);
}

.hotWord {
  margin: 0 auto;
  padding: 5px 0;
  padding-left: 18px;
  width: 350px !important;
}

.list > li {
  float: left;
  list-style: none;
}

.clear {
  clear: both;
}
</style>