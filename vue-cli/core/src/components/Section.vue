<template>
  <section class="section">
    <h1>
      嗨～我是被暴露的組件
    </h1>
    <slot />
  </section>
</template>

<script>
export default {
  name: 'Section',
}
</script>

<style>
.section {
  border: 1px solid black;
  padding: 10px;
  background-color: rgba(0,0,0,0.3);
}
</style>