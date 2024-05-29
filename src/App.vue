<script setup lang="ts">
import { RouterView } from 'vue-router'
import Header from '@/components/global/Header.vue';
import Footer from '@/components/global/Footer.vue';
import moment from 'moment';

const getCurrentDate = () => {
  return moment().format('YYYY-MM-DD');
}
</script>

<template>
  <Header />
  <RouterView />
  <Footer :currentDate="getCurrentDate()" />
</template>


