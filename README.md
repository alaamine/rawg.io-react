#  App React — Explorateur de jeux vidéo

> Projet réalisé en 2025 à **Supinfo Paris** — Projet binôme

##  Description

Application web React utilisant l'API RAWG pour explorer une base de données de jeux vidéo. Recherche, filtres, tri, favoris persistants et accessibilité numérique.

##  Fonctionnalités

-  Recherche de jeux en temps réel
-  Filtres par plateforme (PC, Xbox, PlayStation, etc.) et par store (Steam, Epic, etc.)
-  Tri des résultats selon toutes les options de l'API
-  Pagination / infinite scroll
-  Page détail d'un jeu (nom, description, trailer, plateformes, tags, studios)
-  Achievements avec barre de progression
-  Page éditeur avec tous ses jeux
-  Favoris persistants (Context + localStorage)
-  Page 404 personnalisée
-  Tests end-to-end avec Cypress

##  Technologies utilisées

![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat&logo=axios&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=flat&logo=cypress&logoColor=white)

##  Structure du projet

```
projet-react/
├── src/
│   ├── components/
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── GameDetail.jsx
│   │   ├── Publisher.jsx
│   │   ├── Favorites.jsx
│   │   └── NotFound.jsx
│   ├── context/
│   │   └── FavoritesContext.jsx
│   └── api/
│       └── rawgClient.js
├── cypress/
│   └── e2e/
│       └── games.cy.js
├── .env.example
└── README.md
```

##  Installation

```bash
git clone https://github.com/alaamine/projet-react
cd projet-react
npm install
cp .env.example .env  # Ajouter ta clé API RAWG
npm run dev
```

##  Tests Cypress

```bash
npm run cypress:open
```

##  Ce que j'ai appris

- Développement d'une app React avec hooks et Context API
- Consommation d'une API REST externe avec Axios
- Gestion des favoris persistants avec localStorage
- Isolation des styles CSS (CSS Modules)
- Tests end-to-end avec Cypress
- Accessibilité numérique (a11y)
- Notifications avec react-toastify

---

*Projet académique — Supinfo Paris 2025*
