<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <h1 class="h1 ion-margin">Chats</h1>
      <ion-list class="ion-margin">
        <ion-item router-link="/chat-details">
          <ion-thumbnail>
            <img class="item-image" src="../images/minsk.png" />
          </ion-thumbnail>
          <ion-label class="ion-margin-start">
            <ion-text>
              <h2 class="item-title ion-margin-bottom">
                <strong>Minsk</strong>
              </h2>
              <br />
              <p class="desc">Bob says hi!</p>
            </ion-text>
          </ion-label>
          <ion-label slot="end" class="ion-text-center">
            <span class="desc">12:12</span><br /><br />
            <ion-badge color="primary" class="notification-badge">11</ion-badge>
          </ion-label>
        </ion-item>
        <ion-item>
          <ion-thumbnail>
            <img class="item-image" src="../images/moscow.png" />
          </ion-thumbnail>
          <ion-label class="ion-margin-start">
            <ion-text>
              <h2 class="item-title ion-margin-bottom">
                <strong>Moscow</strong>
              </h2>
              <br />
              <p class="desc">Bob says hi!</p>
            </ion-text>
          </ion-label>
        </ion-item>
        <ion-item>
          <ion-thumbnail>
            <img class="item-image" src="../images/kiev.png" />
          </ion-thumbnail>
          <ion-label class="ion-margin-start">
            <ion-text>
              <h2 class="item-title ion-margin-bottom">
                <strong>Kiev</strong>
              </h2>
              <br />
              <p class="desc">Bob says hi!</p>
            </ion-text>
          </ion-label>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonContent } from "@ionic/vue";
import { useRouter } from "vue-router";

export default {
  name: "chatList",
  components: {
    IonContent,
    IonPage,
  },
  setup() {
    const router = useRouter();
    return { router };
  },
};
</script>