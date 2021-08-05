<template>
  <base-layout pageTitle="Mes souvenirs">
    <ion-list>
        <ion-item router-link="/memories/1">Voyage à l'ile Maurice</ion-item>
        <ion-item>Nager avec des dauphins</ion-item>
        <ion-item>Road trip à Cuba</ion-item>
      </ion-list>
  </base-layout>
</template>

<script>
import { IonList, IonItem} from '@ionic/vue';

export default {
  components: {
    IonList,
    IonItem
  }
}
</script>
