<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
        <ion-card class="Laadpaal-info">
          <ion-card-header>
            <ion-card-title>Laadpalen info</ion-card-title>
          </ion-card-header>
          <ion-card-content>
            <ion-item>
              <ion-label>
                
                <ion-card class="Laadpaal-status">
                  <ion-card-header>
                    <ion-card-title>Laadpaal 1</ion-card-title>
                  </ion-card-header>
                  <ion-card-content>
                    <p class="status-opladen">Status : Opladen</p>
                  </ion-card-content>
                </ion-card>

                <ion-card class="Laadpaal-status">
                  <ion-card-header>
                    <ion-card-title>Laadpaal 2</ion-card-title>
                  </ion-card-header>
                  <ion-card-content>
                    <p class="status-vrij">Status : Vrij</p>
                  </ion-card-content>
                </ion-card>

                <ion-card class="Laadpaal-status">
                  <ion-card-header>
                    <ion-card-title>Laadpaal 3</ion-card-title>
                  </ion-card-header>
                  <ion-card-content>
                    <p class="status-bezet">Status : Bezet</p>
                  </ion-card-content>
                </ion-card>

                <ion-card class="Laadpaal-status">
                  <ion-card-header>
                    <ion-card-title>Laadpaal 4</ion-card-title>
                  </ion-card-header>
                  <ion-card-content>
                    <p class="status-vrij">Status : Vrij</p>
                  </ion-card-content>
                </ion-card>
                
              </ion-label>
            </ion-item>
          </ion-card-content>    
        </ion-card>
    </ion-content>
  </ion-page>
</template>

<script setup>
import { IonContent, IonHeader, IonMenu, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
</script>

<style scoped>
/* ion card klein maken en naar links zetten */
/* alleen laten zien op desktop */
.Laadpaal-info {
  width: 30%;
  text-align: center;
}
/* p moet kleiner zijn */
p{
  font-size: 15px;
}

/* laadpaalstatus moet naast elkaar komen en kleiner gemaakt worden */
.Laadpaal-status {
  width: 40%;
  text-align: center;
  display: inline-block;
  background-color: #2a2727;
}

@-webkit-keyframes charging {
  0% {color: #39FF14;}
  25% {color: #D0F0C0;}
  50% {color: #98FB98;}
  100% {color: #39FF14}
}

.status-opladen {
  animation: charging 5s infinite;
} 
.status-vrij {
  color: green;
}
.status-bezet {
  color: red;
}

</style>
