<template>
	<ion-page>
		<ion-tabs>
			<ion-router-outlet></ion-router-outlet>
			<ion-tab-bar slot="bottom">
				<ion-tab-button href="/tabs/tab1" tab="tab1">
					<ion-icon :icon="triangle" aria-hidden="true" />
					<ion-label>Tab 1</ion-label>
				</ion-tab-button>

				<ion-tab-button href="/tabs/tab2" tab="tab2">
					<ion-icon :icon="ellipse" aria-hidden="true" />
					<ion-label>Tab 2</ion-label>
				</ion-tab-button>

				<ion-tab-button href="/tabs/tab3" tab="tab3">
					<ion-icon :icon="square" aria-hidden="true" />
					<ion-label>Tab 3</ion-label>
				</ion-tab-button>
			</ion-tab-bar>
		</ion-tabs>
	</ion-page>
</template>

<script lang="ts" setup>
import {
	IonIcon,
	IonLabel,
	IonPage,
	IonRouterOutlet,
	IonTabBar,
	IonTabButton,
	IonTabs,
} from '@ionic/vue';
import { ellipse, square, triangle } from 'ionicons/icons';
</script>
