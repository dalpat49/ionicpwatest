
<script lang="ts" setup>
import {ref} from 'vue'
import { IonContent, IonHeader, IonFooter, IonButtons, IonButton, IonPage, IonTitle, IonToolbar, IonFab,IonFabButton,IonIcon, actionSheetController, isPlatform ,IonToast , IonAlert  } from '@ionic/vue';
  

const isshown = ref(false);
const openALAERT  =()=>{
  isshown.value = true
}


const  alertButtons = ['ok done']

</script>



<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Dalpat app</ion-title>
        <ion-buttons >
          <ion-button>
            <ion-icon  name="checkbox"></ion-icon>
            <ion-icon name="checkbox-outline"></ion-icon>
          </ion-button>
        </ion-buttons>
        <ion-buttons >
          <ion-button >
            <ion-icon ios="ellipsis-horizontal" md="ellipsis-vertical"></ion-icon>
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>

    
    <ion-content :fullscreen="true">
      <ion-button  >Disabled</ion-button>
    <ion-button @click="openALAERT" >Click Me</ion-button>
      <ion-alert
        trigger="present-alert"
        v-model="isshown"
        header="Alert"
        sub-header="Important message"
        message="This is an alert!"
        :buttons="alertButtons"
      ></ion-alert>
      <ion-button id="open-toast" expand="block">Open</ion-button>
    <p>This toast example uses triggers to automatically open a toast when the button is clicked.</p>
    <ion-toast trigger="open-toast" message="This toast will disappear after 5 seconds" :duration="5000"></ion-toast>


    </ion-content>
   
  </ion-page>
</template>

<style scoped>
ion-buttons {
  overflow:auto;
}
</style>
