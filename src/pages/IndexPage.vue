<template>
  <q-page class="row items-center justify-evenly">
    <example-component-one model-value="X" />
    <example-component-two model-value="X" />
    <example-component-three model-value="X" />
  </q-page>
</template>

<script setup lang="ts">
import ExampleComponentOne from 'src/components/ExampleComponentOne.vue';
import ExampleComponentTwo from 'src/components/ExampleComponentTwo.vue';
import ExampleComponentThree from 'src/components/ExampleComponentThree.vue';
</script>
