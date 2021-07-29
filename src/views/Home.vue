<template>
  <v-app>
    <v-main>
      <list-client />
    </v-main>
  </v-app>
</template>

<script lang="ts">
  import Vue from 'vue'
  import ListClient from '../components/ListClient.vue';
  export default Vue.extend({
    name: 'Home',

    components: {
      ListClient,
    },
  })
</script>
