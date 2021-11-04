<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <Demo />
    <w-card imgSrc="haizei.jpeg" summary="测试一下">
      <template slot="footer">
        <div class="c">"2021-11-03T13:26:47.452Z"</div>
      </template>
    </w-card>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    // HelloWorldc
  }
};
</script>

<style>
.c {
  font-size: 12px;
  color: #ccc;
  padding-left: 8px;
}
</style>
