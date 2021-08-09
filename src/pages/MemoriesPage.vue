<template>
  <base-layout pageTitle="Mes souvenirs">
    <ion-list>
        <ion-item v-for="memory in memories" :router-link="`/memories/${memory.id}`" :key="memory.id">
        {{ memory.name }}
        </ion-item>
      </ion-list>
  </base-layout>
</template>

<script>
import { IonList, IonItem} from '@ionic/vue';

export default {
  components: {
    IonList,
    IonItem
  },
  data() {
    return{
      memories: [
        {
          id: 1,
          name: "Voyage à l'ile Maurice",
          description: "C'était super !"
        },
        {
          id: 2,
          name: "Nager avec des dauphins",
          description: "L'océan était glaçé"
        },
        {
          id: 3,
          name: "Road trip à Cuba",
          description: "Pour les 50 ans de tata"
        }
      ]
    }
  }
}
</script>
