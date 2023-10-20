
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
      <IonButton  >Disabled</IonButton>
      <h1>dalpat</h1>
    <IonButton @click="openALAERT" >Click Me</IonButton>
      <IonAlert
        :is-open="isshown"
        header="Alert"
        sub-header="Important message"
        message="This is an alert!"
        :buttons="alertButtons"
        @didDismiss="openALAERT"
      ></IonAlert>


    </ion-content>
    
   
  </ion-page>

</template>

<style scoped>
ion-buttons {
  overflow:auto;
}
</style>
