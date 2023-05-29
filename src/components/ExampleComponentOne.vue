<template>
  <q-input v-bind="props">
    <template v-for="(_, slotName) in slots" #[slotName]="slotData">
      <slot :name="slotName" v-bind="slotData" />
    </template>
  </q-input>
</template>

<script setup lang="ts">
import { QInputProps, QInputSlots } from 'quasar';

// eslint-disable-next-line vue/prop-name-casing
const props = defineProps<QInputProps>();
const slots = defineSlots<QInputSlots & { dummy: (scope: string) => void }>();
</script>
