<template>
  <div>
    <button @click="update()">update</button>
    {{response}}
  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: 'Api',
  data() {
    return {
      response: {},
    };
  },
  methods: {
    update() {
      axios.get('https://jsonplaceholder.typicode.com/todos/1')
      // eslint-disable-next-line no-return-assign
        .then(r => this.response = r.data);
    },
  },
};
</script>

<style scoped>

</style>
