
# Jeux à la demande – 10 $ / jeu

Site vitrine **GitHub Pages** pour vendre des mini-jeux sur commande à 10 $/jeu.

## Déploiement

1. Crée un dépôt public et mets `index.html` à la racine.
2. Active **Settings → Pages** → *Branch:* `main`, *Folder:* `/root`.
3. Ouvre l'URL `https://TON-PSEUDO.github.io/NOM-DU-DEPOT`.

## Configuration

Dans `index.html` modifie la section :
```js
window.APP_CONFIG = {
  FORM_ENDPOINT: "https://formspree.io/f/xxxxx",
  PAYPAL_ME: "https://paypal.me/lucasudre/10",
  CONTACT_EMAIL: "luca.sudre@outlook.fr",
  TEST_MODE: false
};
```
