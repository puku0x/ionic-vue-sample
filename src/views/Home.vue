<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <h1>{{title}}</h1>
      <section class="logo">
        <img src="../assets/logo.png" alt="logo" />
      </section>
      <ion-button expand="full" v-on:click="push()">Next</ion-button>
    </ion-content>
  </div>
</template>

<script>
export default {
  name: 'home',
  data: () => {
    return {
      title: 'Home page'
    };
  },
  methods: {
    push() {
      this.$router.push('/about');
    }
  }
};
</script>

<style scoped>
.logo {
  display: flex;
  justify-content: center;
}
</style>