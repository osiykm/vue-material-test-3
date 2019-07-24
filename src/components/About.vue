<template>
  <div class="about">
    <h1>This is an about page</h1>
    <material-component name="Hello"></material-component>
  </div>
</template>
<script>
// @ is an alias to /src
import MaterialComponent from '@/components/About/MaterialComponent.vue';

export default {
  name: 'about',
  components: {
    MaterialComponent,
  },
};
</script>
