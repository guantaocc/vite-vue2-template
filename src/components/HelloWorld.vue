<script>
import { ref, defineComponent } from 'vue'

export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      count: 0,
    }
  },
})
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>

    <p>
      Recommended IDE setup:
      <a href="https://code.visualstudio.com/" target="_blank">VSCode</a>
      +
      <a href="https://marketplace.visualstudio.com/items?itemName=octref.vetur" target="_blank"> Vetur </a>
    </p>

    <p>See <code>README.md</code> for more information.</p>

    <p>
      <a href="https://vitejs.dev/guide/features.html" target="_blank"> Vite Docs </a>
      |
      <a href="https://vuejs.org/" target="_blank">Vue 2 Docs</a>
    </p>

    <button type="button" @click="count++">count is: {{ count }}</button>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
