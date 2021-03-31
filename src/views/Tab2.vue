<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="tertiary">
        <ion-buttons slot="start"
          ><ion-icon
            :icon="menuOutline"
            class="menu-outline ion-padding-start"
          ></ion-icon>
        </ion-buttons>
        <ion-title color="light ion-text-center">Jogjakarta</ion-title>
        <ion-buttons slot="end"
          ><ion-icon
            :icon="calendarOutline"
            class="menu-outline ion-padding-end"
          ></ion-icon>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true" padding>
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-item>
        <ion-label position="floating">Search City</ion-label>
        <ion-input></ion-input>
      </ion-item>

      <ion-grid>
        <ion-row>
          <ion-col>
            <h2 class="ion-text-center">Hourly</h2>
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col> </ion-row
        ><ion-row>
          <ion-col>
            <ion-card>
              <ion-item>
                <ion-label
                  ><p>Tue</p>
                  <p>29/3</p></ion-label
                >
                <ion-icon :icon="rainy" class="rainy"></ion-icon>
              </ion-item>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<script>
import {
  rainyOutline,
  menuOutline,
  calendarOutline,
  thermometerOutline,
  water,
  rainy,
} from "ionicons/icons";

import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonInput,
  IonCol,
  IonRow,
  IonGrid,
  IonIcon,
  IonItem,
  IonCard,
} from "@ionic/vue";

export default {
  data: () => {
    return {};
  },
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonInput,
    IonCol,
    IonRow,
    IonGrid,
    IonIcon,
    IonItem,
    IonCard,
  },
  setup() {
    return {
      rainyOutline,
      menuOutline,
      calendarOutline,
      thermometerOutline,
      water,
      rainy,
    };
  },
};
</script>

<style>
.center {
  margin-left: auto;
  margin-right: auto;
  display: block;
}
ion-card {
  border: 1px solid grey;
}
.rainy {
  font-size: 1.7em;
  color: rgb(76, 175, 175);
}
</style>
