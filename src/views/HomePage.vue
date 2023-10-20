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
    </ion-content>
    <ion-footer >
      <ion-toolbar>
        <ion-buttons>
          <ion-button>
            Select All
          </ion-button>
          <ion-button >
            Deselct All
          </ion-button>
          <ion-button>
            Remove Selected
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-footer>
  </ion-page>
</template>

<script lang="ts" setup>
import { IonContent, IonHeader, IonFooter, IonButtons, IonButton, IonPage, IonTitle, IonToolbar, IonFab,IonFabButton,IonIcon, actionSheetController, isPlatform } from '@ionic/vue';
import Dynamsoft from 'mobile-web-capture';
import { WebTwain } from 'mobile-web-capture/dist/types/WebTwain';
import { DocumentConfiguration } from "mobile-web-capture/dist/types/Addon.Camera";
import { Base64Result } from "mobile-web-capture/dist/types/WebTwain.IO";
import { defineComponent, onMounted, ref } from 'vue';
import DWT from '../components/DWT.vue'
import { createOutline,cameraOutline,saveOutline,checkboxOutline,checkbox,ellipsisHorizontal,ellipsisVertical } from 'ionicons/icons';
import { addIcons } from 'ionicons';
import { ThumbnailViewer } from 'mobile-web-capture/dist/types/WebTwain.Viewer';
import { AndroidPermissions } from '@awesome-cordova-plugins/android-permissions/';
import { Directory, Filesystem } from '@capacitor/filesystem';
import { Capacitor } from "@capacitor/core";
import { Share } from '@capacitor/share';
import { DynamsoftEnumsDWT } from 'mobile-web-capture/dist/types/Dynamsoft.Enum';

  
</script>

<style scoped>
ion-buttons {
  overflow:auto;
}
</style>
