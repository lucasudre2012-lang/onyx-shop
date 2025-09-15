
# Jeux à la demande – 10 $ / jeu

Site vitrine **GitHub Pages** pour vendre des mini‑jeux sur commande à 10 $/jeu.

## Déploiement

1. Crée un dépôt public et mets `index.html` à la racine.
2. Active **Settings → Pages** → *Branch:* `main`, *Folder:* `/root`.
3. Ouvre l'URL `https://TON-PSEUDO.github.io/NOM-DU-DEPOT`.

## Configuration (dans le fichier index.html)

En haut du fichier, modifie :
```js
window.APP_CONFIG = {
  FORM_ENDPOINT: "https://formspree.io/f/xxxxx", // ton endpoint
  PAYPAL_ME: "https://paypal.me/VOTRE_PSEUDO/10",
  CONTACT_EMAIL: "luca.sudre@outlook.fr",
  TEST_MODE: false
};
```

- Si `FORM_ENDPOINT` est vide et `TEST_MODE=false`, la soumission affiche un message d'erreur (sans jeter d'exception).
- Mets `TEST_MODE=true` pour tester localement (les soumissions sont sauvegardées dans `localStorage`).

## Tests

Ajoute `?runTests=1` à l'URL pour lancer les tests du formulaire (affichage en bas à droite).

## Dossier assets

- `assets/logo.png` (optionnel) — logo du site (inclus si disponible).
