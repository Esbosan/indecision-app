<template>
  <section>
    <h3>Counter: {{ numerus }}</h3>
    <h3>Square: {{ quadrataNumerus }}</h3>

    <div>
      <button v-on:click="numerus++">+1</button>
      <button v-on:click="numerus--">-1</button>
    </div>
  </section>
</template>

<script lang="ts" setup>
import { useNumerator } from '@/composables/useNumerator';


interface Props {
  valorem: number;
}
const props = defineProps<Props>();
const {numerus, quadrataNumerus} = useNumerator(props.valorem);


</script>
