<script setup>
import AppCard from '@/components/AppCard.vue';
import AppInput from '@/components/AppInput.vue';
import AppButton from '@/components/AppButton.vue';
import TheMainNav from '@/components/TheMainNav.vue';
import { useDark } from '@vueuse/core'
import Flexbox from '@/components/Flexbox.vue';
import Grid from '@/components/Grid.vue';

const isDark = useDark()
</script>

<template>
  <div class="m-10">
    <input type="checkbox" v-model="isDark" />Dark Mode
    <AppCard />
    <TheMainNav />
    <form action="">
      <label> </label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form>
    <p class="first-letter:text-5xl selection:bg-yellow-400">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Corrupti sequi
      aspernatur deleniti, sed minus vero iusto repudiandae quaerat molestias
      asperiores delectus, quis debitis explicabo voluptatibus. Adipisci quasi
      vero error voluptates?
    </p>
    <ul class="list-disc marker:text-green-500 marker:text-2xl">
      <li>Vue.js</li>
      <li>React</li>
      <li>Svelte</li>
      <li>Solid</li>
    </ul>
    <Flexbox />
    <Grid />
  </div>
</template>
