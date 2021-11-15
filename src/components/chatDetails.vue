<template>
  <ion-page>
    <ion-header class="ion-no-border header-shadow">
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button defaultHref="home" color="primary"></ion-back-button>
        </ion-buttons>

        <ion-row>
          <ion-col size="2">
            <img class="item-image" src="../images/minsk.png" />
          </ion-col>
          <ion-col size="8">
            <ion-lable> Minsk</ion-lable> <br />
            <p
              class="header"
              style="margin-top: 2px; font-size: 14px; color: #707b7c"
            >
              Last message at 13:02
            </p>
          </ion-col>
        </ion-row>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-list>
        <ion-item lines="none">
          <ion-col size="3" class="user-thumb-main">
            <ion-label class="user-thumb-main">
              <ion-thumbnail class="user-thumb">
                <img class="item-image" src="../images/user-img.png" />
              </ion-thumbnail>
            </ion-label>
          </ion-col>
          <ion-col size="9">
            <ion-label class="ion-text-end chat-content">
              <img class="item-image" src="../images/cat.png" />
              <ion-label>
                <p class="chat-text ion-text-wrap">
                  Hi I Just Knocked you a while ago.
                </p>
                <h2 class="text-time">12:12</h2>
              </ion-label>
            </ion-label>
          </ion-col>
        </ion-item>
        <br />
        <ion-item lines="none">
          <ion-col size="3" class="user-thumb-main">
            <ion-label class="user-thumb-main">
              <ion-thumbnail class="user-thumb">
                <img class="item-image" src="../images/minsk.png" />
              </ion-thumbnail>
            </ion-label>
          </ion-col>
          <ion-col size="9">
            <ion-label class="ion-text-end chat-content">
              <ion-label>
                <p class="chat-text ion-text-wrap">
                  Hi I Just Knocked you a while ago.
                </p>
                <h2 class="text-time">12:12</h2>
              </ion-label>
            </ion-label>
          </ion-col>
        </ion-item>
      </ion-list>

      <div class="input-area">
        <ion-item lines="none" class="mic-attach-main">
          <ion-icon
            class="ion-text-center mic-attach-icons"
            :icon="attach"
          ></ion-icon>
          <span class="space-between"></span>
          <ion-icon
            class="ion-text-center mic-attach-icons"
            :icon="mic"
          ></ion-icon>
        </ion-item>
        <div class="input-message">
          <form name="messageForm">
            <ion-item>
              <ion-input
                type="text"
                name="message"
                id="message"
                placeholder="Type your message..."
              ></ion-input>
            </ion-item>

            <!-- <button>
            <ion-icon name="send"></ion-icon>
          </button> -->
          </form>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonContent } from "@ionic/vue";
import { mic, attach } from "ionicons/icons";

export default {
  name: "chatDetails",
  components: {
    IonContent,
    IonPage,
  },
  setup() {
    return {
      mic,
      attach,
    };
  },
};
</script>