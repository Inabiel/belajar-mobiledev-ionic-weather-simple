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
            <center>
              <h2 class="ion-text-center">6.20 PM</h2>
              <ion-icon :icon="rainyOutline" class="iconrain"></ion-icon>
              <h3 class="ion-text-center">The Weather is Now</h3>
              <h1 class="ion-text-center">Rainy</h1>
            </center>
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col sizeSm="12" sizeLg="3" offsetLg="4.5">
            <center>
              <ion-list list="full">
                <ion-item>
                  <ion-icon
                    :icon="thermometerOutline"
                    class="thermo-outline"
                  ></ion-icon>
                  <ion-label>1920 Hpa </ion-label>
                  <ion-icon :icon="water" class="water"></ion-icon>
                  <ion-label> 93% </ion-label>
                  <ion-icon :icon="rainy" class="rainy"></ion-icon>
                  <ion-label no-lines>Mau ujan</ion-label>
                </ion-item>
              </ion-list>
            </center>
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col>
            <h2 class="ion-text-center">Tomorrow</h2>
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
  name: "Tab1",
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
.iconrain {
  color: blue;
  font-size: 13em;
}
.menu-outline {
  color: white;
  font-size: 1.8em;
}
h1 {
  font-size: 3em;
}
.thermo-outline {
  font-size: 1.7em;
  color: red;
}
.water {
  font-size: 1.7em;
  color: blue;
}
.rainy {
  font-size: 1.7em;
  color: rgb(76, 175, 175);
}
.center {
  margin-left: auto;
  margin-right: auto;
  display: block;
}
ion-card {
  border: 1px solid grey;
}
</style>
