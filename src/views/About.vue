<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button defaultHref="/"></ion-back-button>
        </ion-buttons>
        <ion-title>About</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <h1>{{title}}</h1>
      <ion-button expand="full" v-on:click="pop()">Prev</ion-button>
    </ion-content>
  </div>
</template>

<script>
export default {
  name: 'about',
  data: () => {
    return {
      title: 'About page'
    };
  },
  methods: {
    pop() {
      this.$router.go(-1);
    }
  }
};
</script>
