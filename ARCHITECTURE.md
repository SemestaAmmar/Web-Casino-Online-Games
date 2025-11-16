# Architecture du projet Casino Web

## Structure du projet

```
web_casino_online_games/
│
├─ index.html # Page principale HTML
├─ css/
│ └─ style.css # Styles globaux et spécifiques aux jeux
├─ js/
│ └─ main.js # Scripts JS pour les jeux et gestion du solde
├─ README.md
├─ INSTALL.md
├─ ARCHITECTURE.md
├─ CHANGELOG.md
├─ CONTRIBUTING.md
├─ LICENSE
└─ ROADMAP.md
```


## Modules principaux

- `index.html` :
  - Structure HTML globale du casino
  - Header avec solde
  - Menu de sélection des jeux
  - Conteneur dynamique pour charger les jeux

- `css/style.css` :
  - Styles globaux pour le body, header, footer
  - Styles des boutons et contrôles
  - Styles spécifiques aux jeux : roulette, slots, blackjack
  - Animations et transitions pour les éléments interactifs

- `js/main.js` :
  - Gestion du solde et des mises
  - Roulette complète avec animation et historique
  - Machine à sous avec symboles animés et calcul des gains
  - Blackjack complet avec cartes animées et calcul de score
  - Gestion du menu de sélection des jeux et mise à jour dynamique du conteneur

## Flux de l'application

1. L'utilisateur ouvre le navigateur et charge `index.html`.
2. Le solde initial est affiché.
3. L'utilisateur sélectionne un jeu via le menu.
4. Le jeu choisi s'affiche dynamiquement dans le conteneur.
5. L'utilisateur place sa mise et joue.
6. Les gains ou pertes sont automatiquement calculés et appliqués au solde.
7. L'utilisateur peut rejouer autant de fois qu'il le souhaite.

## Technologies utilisées

- HTML5, CSS3, JavaScript ES6
- Canvas pour la roulette
- Animations CSS et JS pour les cartes et les rouleaux
- Standard Web API pour manipulation DOM et événements

## Concepts clés

- Solde virtuel mis à jour en temps réel
- Jeux interactifs avec animations et transitions
- Calcul automatique des gains selon les règles de chaque jeu
- Gestion propre et modulable de chaque jeu
