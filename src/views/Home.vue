<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar class="pl" color="secondary">
        <ion-title>Carlos-App</ion-title>
      </ion-toolbar>
      <ion-toolbar>
            <ion-searchbar color="primary"></ion-searchbar>
      </ion-toolbar>
    </ion-header>
    
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar >
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>
      <div class="cible"><span></span></div>
      <ion-item>
            <ion-label>Nom:</ion-label>
            <ion-input placehoder="your name"></ion-input>
      </ion-item>
        <ion-item>
        <ion-label>prenom:</ion-label>
            <ion-input placehoder="your name"></ion-input>
        </ion-item>
           <ion-item>
           <ion-label>postnom:</ion-label><br>
            <ion-input placehoder="your" expand="block"></ion-input>
          </ion-item>
        <ion-button >Valider</ion-button>

    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar
  }
});
</script>

<style scoped>
.cible{
  width:20px;
  background-color:red;
  height:10px;
  position:absolute;
  top:100px;
  right:200px;
  z-index:5;
}
</style>