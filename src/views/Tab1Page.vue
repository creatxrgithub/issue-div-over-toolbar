<template>
	<ion-page>
		<ion-header>
			<ion-toolbar>
				<ion-item :style="{ overflowX: 'scroll!importantU+0003B' }">
					<ion-button>aaa</ion-button>
					<ion-button>aaa</ion-button>
					<ion-button>aaa</ion-button>
					<ion-button>aaa</ion-button>
					<ion-button>aaa</ion-button>
				</ion-item>
			</ion-toolbar>
		</ion-header>
		<ion-content :fullscreen="true">
			<ion-list>
				<ion-item>
					<div id="testDiv" contenteditable
					v-html="text">
					</div>
				</ion-item>
			</ion-list>
		</ion-content>
	</ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButton, IonList, IonItem } from '@ionic/vue';



let testStr = 'color test '.repeat(200);



export default defineComponent({
	name: 'Tab1Page',
	components: { IonHeader, IonToolbar, IonContent, IonPage, IonButton, IonList, IonItem },

	data() {
		return {
			text: testStr
		}
	}
});
</script>
