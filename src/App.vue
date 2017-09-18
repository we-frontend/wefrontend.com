<template>
  <div>
    <wf-nav />
    <wf-main />
  </div>
</template>

<script>
  import wfMain from './components/main/main.vue';
  import wfNav from './components/navigation/navigation.vue';

  export default {
      components: {
          wfMain,
          wfNav
      }
  }
</script>

<style lang="scss" src="./App.scss"></style>
