<template>
  <Suspense>
    <template #default>
      <main>
        <h1>Vue 3 Suspense fetch API</h1>
        <PostList />
      </main>
    </template>
    <template #fallback>Loading... </template>
  </Suspense>
</template>

<script>

import PostList from "./components/PostList.vue";
export default {
  name: "App",
  components: {
    PostList
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
}
body {
  background-color: #2c3e50;
  padding: 20px;
}
</style>
