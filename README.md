# Ma collection de DVD

Application web (PWA) pour gérer une collection de DVD : ajout, modification,
recherche, scan de code-barre, export/import Excel, installable sur mobile.

## Fichiers

- `index.html` — l'application
- `manifest.json` — définit le nom, l'icône et le mode d'affichage de l'app
- `sw.js` — service worker minimal (nécessaire pour que Chrome propose une
  vraie installation, et pas seulement un raccourci sur l'écran d'accueil)
- `icon-192.png`, `icon-512.png`, `icon-180.png` — icônes de l'application

## Installation sur GitHub Pages

1. Crée un dépôt GitHub et mets-y tous ces fichiers (à la racine)
2. Settings → Pages → Branch: main / (root) → Save
3. Ouvre le lien `https://TON-NOM.github.io/TON-DEPOT/` dans Chrome (Android)
4. Utilise le bouton « ⬇️ Installer » dans l'app, ou le menu ⋮ → « Installer
   l'application »

Grâce au manifeste et au service worker en fichiers séparés (au lieu
d'être intégrés dans le HTML), Chrome devrait proposer une installation
complète, qui place l'app dans le tiroir d'applications et dans
Paramètres → Applications, comme n'importe quelle autre app.
