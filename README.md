[README.md](https://github.com/user-attachments/files/32146225/README.md)
# ZEN — PWA

ZEN est une PWA statique pensée pour GitHub Pages. Elle fonctionne sans backend : les notes, projets, citations, thème, langue et fond personnalisé sont stockés localement dans le navigateur.

## Déployer sur GitHub Pages

1. Crée un repository GitHub, par exemple `ZEN`.
2. Décompresse ce ZIP.
3. Envoie **le contenu du dossier ZEN** à la racine du repository : `index.html`, `css/`, `js/`, `assets/`, etc.
4. Dans GitHub : **Settings → Pages → Deploy from a branch**.
5. Sélectionne la branche `main` et le dossier `/ (root)`.
6. Ouvre l'URL GitHub Pages fournie par GitHub.

> Le service worker et le mode installable PWA fonctionnent sur HTTPS, donc GitHub Pages convient.

## Fonctionnalités

- Écran de lancement Z + paillettes.
- Accueil avec montre analogique temps réel.
- Notes avec 7 dernières notes, filtre « idée importante » et favoris importants.
- Projets avec création de dossiers, notes et photo.
- Motivation avec citations personnalisées.
- Mode ZEN plein écran avec montre et heure.
- Réglages : Dark/Light, FR/EN, fond d'écran personnalisé.
- Données persistantes via `localStorage`.
- Service worker pour le fonctionnement hors ligne après le premier chargement.

## Important — montres

Les photos de montres fournies sont des références visuelles. Les cadrans de ZEN sont reconstruits en HTML/CSS et les aiguilles sont animées en JavaScript à partir de l'heure réelle. Cela permet aux aiguilles de tourner réellement au lieu de rester figées comme sur une photo.

## Limite volontaire

Les « montres » sont une reproduction graphique inspirée des références, pas un fichier CAO ou un rendu photoréaliste pixel-par-pixel. Le but est d'avoir un rendu cohérent, léger et réellement animé dans une PWA sans dépendance externe.
