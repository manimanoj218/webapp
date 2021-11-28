<template>
  <el-menu
    :default-active="'/'"
    class="el-menu-demo"
    mode="horizontal"
    @select="handleSelect"
    background-color="#545c64"
    text-color="#fff"
    :router="true"
    active-text-color="#ffd04b"
  >
    <el-menu-item index="/">Home</el-menu-item>   
    <el-menu-item index="/about">About</el-menu-item>
  </el-menu>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      activeIndex2: "1",
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style>
</style>