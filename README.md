# GameBox Multi-Emulator

Cette version utilise `www/index.html` comme interface principale.

## Ce qui est réellement intégré
- Interface GameBox.
- Bibliothèque de jeux.
- Sélection de backend par extension.
- Émulation rétro via EmulatorJS/WebAssembly pour les systèmes compatibles.
- Architecture prévue pour des backends Android natifs.

## Ce qui nécessite un moteur natif
Un APK ne peut pas devenir à lui seul un émulateur universel en ajoutant du HTML.
Les jeux Android, Windows et Switch nécessitent des moteurs compatibles distincts, leurs bibliothèques natives et, selon le système, des composants système/licences propres.

Les jeux et ROM doivent être ceux que tu as légalement le droit d'utiliser.

## Compilation
1. Installer Node.js et Android Studio.
2. Installer Android SDK, NDK et CMake.
3. `npm install`
4. `npx cap add android`
5. `npx cap sync android`
6. `npx cap open android`
7. Android Studio > Build > Build APK(s)

Le dossier `android-native/` sert de point d'intégration pour les bibliothèques natives futures.


## Compilation sans PC
Le workflow `.github/workflows/build-apk.yml` compile automatiquement un APK avec GitHub Actions. Voir `INSTALLATION_SANS_PC.md`.
