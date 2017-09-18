<template>
  <div>
    <main class="init-view horizontal">
      <div class="init-view__container vertical">
        <transition name="fade">
          <div class="init-view__content" v-if="show">
            <p class="init-view__logo" :class="{scale : scale}">WE FRONTEND</p>
            <p class="init-view__message">
              <span class="init-view__schedule">[ Box-model & Grid-System ]</span>
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
              show: false,
              scale : false
          }
      },
      methods: {
          initShow() {
              this.show = !this.show;
              setTimeout(()=> {
                  this.scale = !this.scale;
              }, 100);
          }
      },
      mounted() {
          this.initShow();
      }
  }
</script>

<style lang="scss" src="./main.scss" scoped></style>
