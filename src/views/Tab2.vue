<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <chatList name="Tab 2 page" />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonContent } from "@ionic/vue";
import chatList from "@/components/chatList.vue";

export default {
  name: "Tab2",
  components: {
    chatList,
    IonContent,
    IonPage,
  },
};
</script>