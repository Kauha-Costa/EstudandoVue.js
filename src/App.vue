<script setup>
import Layout from './components/layouts/Layout.vue';
import Dashboard from './components/pages/Dashboard.vue';
import Welcome from './components/pages/Welcome.vue';
import Workout from './components/pages/Workout.vue';
import { ref } from 'vue';
import { workoutProgram } from './utils';

const defaultData = {}
//for(let workoutIdx in workoutProgram){
  //const workout = workoutProgram[workoutIdx];

  //defaultData[workoutIdx] = {}

  //for (let e of )

//}
const selectedDisplay = ref(3);
const data = ref();
const selectedWorkout = ref(-1);
</script>

<template>
  <Layout>
    <!-- PAGE 1 -->
    <Welcome v-if="selectedDisplay == 1"/>
    <!-- PAGE 2 -->
    <Dashboard v-if="selectedDisplay == 2"/>
    <!-- PAGE 3 -->
    <Workout v-if="selectedDisplay == 3"/>
  </Layout>
</template>

<style scoped>

</style>
