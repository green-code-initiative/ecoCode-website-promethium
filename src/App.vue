<script setup lang="ts">
import { RouterView } from 'vue-router'
import Header from '@/components/global/Header.vue';
import Footer from '@/components/global/Footer.vue';
import { format } from 'date-fns';

const getCurrentDate = () => {
  return format(new Date(), 'yyyy-MM-dd');
}

</script>

<template>
  <Header />
  <RouterView />
  <Footer :currentDate="getCurrentDate()" />
</template>


