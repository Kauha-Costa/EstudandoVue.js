<script setup>
import Layout from './components/layouts/Layout.vue';
import Dashboard from './components/pages/Dashboard.vue';
import Welcome from './components/pages/Welcome.vue';
import Workout from './components/pages/Workout.vue';

const selectedDisplay = 1;
</script>

<template>
  <Layout>
    <!-- PAGE 1 -->
    <Welcome />
    <!-- PAGE 2 -->
    <Dashboard/>
    <!-- PAGE 3 -->
    <Workout/>
  </Layout>
</template>

<style scoped>

</style>
