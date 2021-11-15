<template>
  <ion-page>
    <ion-content>
      <ion-row>
        <ion-col size="6">
          <h1 class="page-title ion-margin">My profile</h1>
        </ion-col>
        <ion-col size="4"></ion-col>
        <ion-col size="2" class="ion-text-center">
          <ion-icon
            :icon="create"
            class="icon-edit tab-icon"
            size="large"
          ></ion-icon>
        </ion-col>
      </ion-row>
      <ion-label>
        <ion-row>
          <ion-col offset="3.5"> </ion-col>
          <ion-col size="4">
            <img class="img" src="../images/user-img.png" />
            <p class="paragraph">id5</p>
            <h1 class="user-name">Helen Jobs</h1>
            <p class="paragraph">19 year</p>
          </ion-col>
          <ion-col offset="3.5"> </ion-col>
        </ion-row>
      </ion-label>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonContent } from "@ionic/vue";
import { create } from "ionicons/icons";

export default {
  name: "Tab3",
  components: {
    IonContent,
    IonPage,
  },
  setup() {
    return {
      create,
    };
  },
};
</script>