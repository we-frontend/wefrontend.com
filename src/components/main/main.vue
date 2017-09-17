<template>
  <div>
    <main class="init-view horizontal">
      <div class="init-view__container vertical">
        <transition name="fade">
          <div class="init-view__content" v-if="show">
            <p class="init-view__logo">WE FRONTEND</p>
            <p class="init-view__message">
              Coming Soon...
            </p>
            <p class="init-view__github">
              <a href="https://github.com/we-frontend"><i class="fa fa-github-square icon" aria-hidden="true"></i></a>
            </p>
          </div>
        </transition>
      </div>
    </main>
  </div>
</template>

<script>
  export default {
      name: 'main',
      data() {
          return {
              show: false
          }
      },
      methods: {
          initShow() {
              this.show = !this.show;
          }
      },
      mounted() {
          this.initShow();
      }
  }
</script>

<style lang="scss" src="./main.scss" scoped></style>
