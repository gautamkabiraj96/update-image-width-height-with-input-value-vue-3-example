<template>
  <div>
    <h3>Vue 3 change image width and height with input values</h3>
    <input type="number" v-model="imageWidth" inputmode="numeric" />
    <input type="number" v-model="imageHeight" inputmode="numeric" />
    <div class="np-img-container">
      <img
        src="https://picsum.photos/id/1/500/400"
        :style="{
          height: `${imageHeight}px`,
          width: `${imageWidth}px`,
        }"
      />
    </div>
    <!--
      www.nightprogrammer.com
    -->
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      imageWidth: 500,
      imageHeight: 400,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.np-img-container {
  margin: 20px 0;
}
</style>
