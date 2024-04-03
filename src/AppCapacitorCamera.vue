<template>
      <ion-page id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-title>Capacitor Plugins</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
          <img :src="imageURL"/>
          <button @click="makePhoto">Take photo</button>
        </ion-content>
     </ion-page>
</template>
<script setup lang="ts">
import {IonPage,IonToolbar,IonHeader,IonTitle,IonContent} from '@ionic/vue';
import { Camera,CameraResultType } from '@capacitor/camera';
import {ref} from 'vue'
const imageURL=ref()
const makePhoto=async ()=> {
  const image=await Camera.getPhoto({
    quality:100,
    allowEditing:true,
    resultType:CameraResultType.Uri
  })
  imageURL.value=image.webPath
}
</script>
<style></style>

  