<template>
  <div class="q-pa-md q-gutter-sm">
    <input v-model="message" type="text" />
    <q-card>
      <div v-for="mas in arrayMassage" :key="mas">{{ mas }}</div>
    </q-card>
    <q-btn color="secondary" label="Secondary" @click="addContent" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import { Root } from './posts';

export default defineComponent({
  name: 'ExampleComponent',
  data() {
    return {
      message: '',
      arrayMassage: [''],
    };
  },
  mounted() {
    const a: Root = {
      userId: 12,
      id: 23,
      title: 'qweqweqw',
      completed: true,
    };
    console.log(a);
  },
  methods: {
    addContent() {
      this.arrayMassage.push(this.message);
      console.log(this.message, this.arrayMassage);
    },
  },
});
</script>
