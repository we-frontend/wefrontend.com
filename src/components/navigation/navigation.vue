<template>
  <div class="nav">
    <span class="nav__element" @mouseover="showToast">Articles</span>
    <span class="nav__toast">준비 중</span>
    <a href="https://goo.gl/forms/Mx552eDPsnCSl2lz2">
      <span class="nav__element">Join us</span>
    </a>
  </div>
</template>

<script>
  export default {
    name: 'nav'
  }
</script>

<style lang="scss" src="./navigation.scss"></style>
