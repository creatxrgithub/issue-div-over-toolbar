It seems that it's issue for ver6.

when click at the middle height of div and middle position of string, the div over the toolbar.

after upgrade to ver7 in project use the command below, it has no longer toolbar problem.

```
npm install vue@latest vue-router@latest
npm install @ionic/core@7 @ionic/vue@7 @ionic/vue-router@7
``


but after upgraded, it has other problem:
```
<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-item>
          <ion-button>AAA</ion-button>
          <ion-button>AAA</ion-button>
          <ion-button>AAA</ion-button>
          <ion-button>AAA</ion-button>
          <ion-toggle>TTT</ion-toggle>
        </ion-item>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 2</ion-title>
        </ion-toolbar>
      </ion-header>

    </ion-content>
  </ion-page>
</template>
```
with the code above, it has a display problem: the button and toggle cannot keep in a same line.

![ver6](issue_images/toggle_with_button_1.png)
![ver7](issue_images/toggle_with_button_2.png)
