<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
    <button @click="changeName('Zelda'), changeAge(30)">Change Name And Age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {},
  data() {
    return {
      name: 'Link',
      age: 25 as number | string
    };
  },
  methods: {
    changeName(name: string) {
      this.name = name;
      return name;
    },

    changeAge(age: number | string) {
      this.age = age;
      return age;
    }
  }
});

</script>

<style>

</style>
