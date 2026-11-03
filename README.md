# 🍼 Biberons — suivi du lait d'un nourrisson

Petite application web installable (PWA) pour noter les millilitres de lait pris par bébé.
Elle fonctionne **hors ligne** et garde les données **uniquement sur votre téléphone** (aucun serveur, aucun compte).

## Fonctions

- Ajout en un geste (60 / 90 / 120 / 150 / 180 ml) avec bouton **Annuler**
- Saisie précise : quantité (+/−), type de lait (infantile, maternel tiré, mixte), date/heure, note
- Total du jour avec jauge d'objectif, nombre de biberons, moyenne par prise, intervalle moyen
- Temps écoulé depuis le dernier biberon
- Navigation jour par jour pour corriger ou rattraper un oubli
- Historique 7 / 14 / 30 jours (graphique + détail par jour)
- Objectif indicatif calculé à partir du poids (≈ 150 ml/kg/jour), modifiable
- Export CSV (tableur) et sauvegarde / import JSON
- Thème clair/sombre automatique

> Ce n'est pas un dispositif médical : les repères affichés sont indicatifs, à valider avec votre pédiatre.

## Déploiement sur GitHub Pages

1. Créez un dépôt GitHub (par ex. `biberons`), public.
2. Envoyez-y **tous les fichiers de ce dossier** à la racine (`index.html`, `manifest.webmanifest`, `sw.js`, les 3 icônes `.png`, `README.md`).
   Sur github.com : *Add file → Upload files*, glissez les fichiers, puis *Commit changes*.
3. Dans le dépôt : **Settings → Pages**.
4. *Source* : **Deploy from a branch** — branche **main**, dossier **/ (root)** — puis *Save*.
5. Après 1 à 2 minutes, l'adresse apparaît : `https://VOTRE-NOM.github.io/biberons/`

## Installation sur Android

1. Ouvrez l'adresse ci-dessus dans **Chrome** sur le téléphone.
2. Menu **⋮ → Installer l'application** (ou *Ajouter à l'écran d'accueil*).
   Vous pouvez aussi utiliser le bouton « Installer l'application » dans l'onglet Réglages.
3. L'icône 🍼 apparaît sur l'écran d'accueil et l'app s'ouvre en plein écran, même sans réseau.

## À savoir

- Les données sont stockées dans le navigateur du téléphone : **ne désinstallez pas / ne videz pas les données de Chrome** sans avoir fait une sauvegarde (*Réglages → Sauvegarde complète*).
- Pour passer d'un téléphone à un autre : exportez le JSON, puis importez-le sur l'autre appareil.
- Pour publier une mise à jour, modifiez les fichiers sur GitHub et changez le numéro `CACHE = 'biberons-v1'` dans `sw.js` (par ex. `biberons-v2`).
