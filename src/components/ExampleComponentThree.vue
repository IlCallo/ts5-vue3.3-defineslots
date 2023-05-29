<template>
  <q-select v-bind="props">
    <template v-for="(_, slotName) in slots" #[slotName]="slotData">
      <slot :name="slotName" v-bind="slotData" />
    </template>
  </q-select>
</template>

<script setup lang="ts">
import { QSelectProps, QSelectSlots } from 'quasar';

// eslint-disable-next-line vue/prop-name-casing
const props = defineProps<QSelectProps>();
const slots = defineSlots<QSelectSlots>();
</script>
