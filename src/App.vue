<template>
  <q-layout id="q-app" view="lHh Lpr lFf">
    <q-page-container>
      <HelloWorld />
    </q-page-container>
  </q-layout>


</template>

<script>
  import {
    openURL
  } from 'quasar'
  import HelloWorld from './components/HelloWorld.vue'

  export default {
    name: 'LayoutDefault',
    components: {
      HelloWorld
    },
    data() {
      return {
        leftDrawerOpen: this.$q.platform.is.desktop
      }
    },
    methods: {
      openURL
    }
  }
</script>

<style>
</style>