<template>
  <q-page-container>
    <Test />
  </q-page-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Test from 'components/Test.vue';

export default defineComponent({
  name: 'App',
  components: {
    Test,
  },
  data() {
    return {
      postsId: {},
    };
  },
});
</script>
