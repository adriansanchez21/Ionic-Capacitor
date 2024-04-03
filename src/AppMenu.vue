<template>
      <ion-menu content-id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-title>
                    Exemple de menú
                </ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content>
            Hola Mon!
        </ion-content>
      </ion-menu>
      <ion-page id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-buttons slot="start">
                    <ion-menu-button></ion-menu-button>
                </ion-buttons>
                <ion-title>Menú</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            <ion-grid>
    <ion-row>
      <ion-col>1</ion-col>
      <ion-col>2</ion-col>
      <ion-col>3</ion-col>
      <ion-col>4</ion-col>
      <ion-col>5</ion-col>
      <ion-col>6</ion-col>
    </ion-row>
  </ion-grid>
        </ion-content>

      </ion-page>
  </template>
  
  <script setup lang="ts">
  import {IonApp,IonPage,IonButtons,IonMenu,IonToolbar,IonHeader,IonMenuButton,IonTitle,IonContent} from '@ionic/vue';
  </script>
  <style scoped>
    ion-col {
    background-color: #135d54;
    border: solid 1px #fff;
    color: #fff;
    text-align: center;
  }
  </style>
  