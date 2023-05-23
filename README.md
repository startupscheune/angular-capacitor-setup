# angular-capacitor-setup
Setup für ein Standard-Projekt mit Angular 15 und Capacitor

## Setup

1. Angular 15 installieren
- https://angular.io/guide/setup-local
- node 18.12.1 LTS https://nodejs.org/dist/v18.12.1/node-v18.12.1-x64.msi
- typescript 4.8.4 `npm install -g typescript@4.8.4`
- angular 15.0.4 `npm install -g @angular/cli@15.0.4`

2. Projekt erstellen mit `ng new deine-app`
   1. routing hinzufügen
   2. CSS als Stylesheet
   3. Test mit `cd my-app` und `ng serve --open`

3. Capacitor hinzufügen: https://capacitorjs.com/solution/angular
   1. `ng add @capacitor/angular` In diesem Projekt Version 2.0.3
      1. Package ID vergeben: com.deinappname.app (Keine Bindestriche)
      2. Join Ionic / Share usage data -> n
   2. `ng build`
   3. Native ios und android installieren `npm i @capacitor/ios @capacitor/android`
      1. `npx cap add android` erstellt Android Projekt -> Mehr dazu: https://capacitorjs.com/docs/basics/workflow
      2. `npx cap add ios` erstellt ios Projekt

4. Android Studio und Xcode herunterladen
- Android: https://developer.android.com/studio
- Xcode (nur unter macOS): https://capacitorjs.com/docs/getting-started/environment-setup#ios-requirements

5. Beispiele für capacitor API
   1. Geolocation: https://capacitorjs.com/docs/apis/geolocation
      1. `npm install @capacitor/geolocation`
      2. `npx cap sync`

## Alles weitere behandeln wir im Workshop
