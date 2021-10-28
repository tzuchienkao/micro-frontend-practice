<template>
  <div id="app">
    <h4>
      &lt;start&gt; 我是組合引用的版 &lt;/start&gt;
    </h4>
    <Section>
      <Button>我是引用被暴露的按鈕</Button>
      <br />
    </Section>
    <p>
      &lt;end&gt; 我是組合引用的版 &lt;/end&gt;
    </p>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    Button: () => import("core/Button"),
    Section: () => import("core/Section"),
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
</style>
