<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <homeComponent name="Tab 1 page" />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonContent } from "@ionic/vue";
import homeComponent from "@/components/homeComponent.vue";

export default {
  name: "Tab1",
  components: {
    homeComponent,
    IonContent,
    IonPage,
  },
};
</script>