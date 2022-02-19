<template>
  <div>
    <app-header v-bind:propsData="headerText" v-on:renew="renewHeaderText"></app-header>
    {{ str }}
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  data: function() {
    return {
      str: 'hi',
      headerText: 'header'
    }
  },
  components: {
    AppHeader
  },
  methods: {
    renewHeaderText() {
      this.headerText = 'new header';
    }
  }
}
</script>

<style>

</style>