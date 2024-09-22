<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button class="cod" type="button" @click="count++">Count is {{ count }}</button>
    <p>
      Edit
      <code class="code">./src/components/hello-world.vue</code> to test Hmr
    </p>
  </div>

  <p>
    Check out
    <a class="link" href="https://vuejs.org/guide/quick-start.html#local" target="_blank">Create-Vue</a>, the official Vue + Vite
    starter
  </p>
  <p>
    Install
    <a class="link" href="https://github.com/vuejs/language-tools" target="_blank">Vue</a>
    in your Ide for a better Dx
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
.cod{
  margin: 0.5rem;
  padding: 0.5rem;
  background-color: #292f31;
  color: rgb(99, 202, 168);
  font-size: large;
  font-weight: bold;
  border-radius: 0.5rem;
}
.code{
  margin: 0.5rem;
  padding: 0.5rem;
  background-color: #292f31;
  color: rgb(153, 223, 162);
  font-size: large;
  font-weight: bold;
  border-radius: 0.5rem;
}
.link{
  margin: 0.2rem;
  padding: 0.2rem;
  color: #99dfa2;
}
</style>