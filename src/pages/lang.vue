<template>
  <div><h1>333333333333</h1>
  <test/>
  </div>
</template>

<script lang="ts">
import { defineComponent, defineAsyncComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {
    test: defineAsyncComponent(() => import('components/test.vue'))
  },
});
</script>
