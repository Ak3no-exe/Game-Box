# INSTALLER GAMEBOX — SANS PC

## 1. Créer le dépôt GitHub
Depuis ton téléphone :
- ouvre GitHub ;
- crée un nouveau dépôt ;
- mets-le en Public ou Private ;
- nom conseillé : `GameBox-MultiEmulator`.

## 2. Envoyer les fichiers
Décompresse ce ZIP si nécessaire et envoie les fichiers du projet dans le dépôt.
Le dossier `.github/workflows/build-apk.yml` doit absolument être présent.

## 3. Lancer la compilation
Dans le dépôt GitHub :
- ouvre l'onglet `Actions` ;
- sélectionne `Build GameBox APK` ;
- appuie sur `Run workflow` ;
- attends la fin du build.

## 4. Récupérer l'APK
Quand le workflow est terminé :
- ouvre l'exécution terminée ;
- descends jusqu'à `Artifacts` ;
- télécharge `GameBox-APK` ;
- ouvre l'archive téléchargée ;
- récupère `app-debug.apk`.

## 5. Installer
Ouvre `app-debug.apk` sur ton téléphone.
Android peut demander l'autorisation d'installer cette application depuis cette source.

## Important
Cette compilation transforme l'interface GameBox en application Android.
Elle ne crée pas automatiquement des moteurs d'émulation Android/Windows/Switch.
Les moteurs natifs correspondants doivent encore être intégrés séparément.
Les jeux/ROM utilisés doivent être ceux que tu as légalement le droit d'utiliser.
