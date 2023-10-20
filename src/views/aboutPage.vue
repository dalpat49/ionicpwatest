
<script lang="ts" setup>
import {ref} from 'vue'
import { IonContent, IonHeader, IonFooter, IonButtons, IonButton, IonPage, IonTitle, IonToolbar, IonFab,IonFabButton,IonIcon, actionSheetController, isPlatform ,IonToast , IonAlert ,IonLabel,   IonTabs ,IonTabBar, IonTabButton } from '@ionic/vue';
  
import { calendar, informationCircle, map, personCircle } from 'ionicons/icons';
const isshown = ref(false);
const openALAERT  =()=>{
  if(isshown.value == false){
    isshown.value = true

  }
  else{
    isshown.value = false

  }
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
      <!-- <IonButton  >Disabled</IonButton> -->
      <h1>Abou page</h1>
      <ion-list>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        <ion-item>
            <ion-label>Item Label</ion-label>
        </ion-item>
        </ion-list>


    </ion-content>
    
   
  </ion-page>

</template>

<style scoped>
ion-buttons {
  overflow:auto;
}
</style>
