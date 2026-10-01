# Architecture

```text
GameBox UI (HTML/CSS/JS)
        |
        +-- Retro / WebAssembly
        |
        +-- Android native backend
        |
        +-- Windows compatibility backend
        |
        +-- Switch backend
        |
        +-- File / save / controller manager
```

Le moteur Android Emulator officiel utilise QEMU, ce qui montre pourquoi
un véritable environnement Android est un composant natif et non une simple
fonction JavaScript. GameBox ne copie pas cet émulateur : il prévoit un
backend natif séparé.
