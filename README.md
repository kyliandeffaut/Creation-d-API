# Création d’une API avec Node.js & TypeScript

## Description
Ce projet est une API simple réalisée avec **Node.js**, **Express** et **TypeScript**
L’API permet de gérer une ressource d’utilisateurs avec des routes basiques : récupération et ajout.

---

## Technologies utilisées
- [Node.js]
- [Express]
- [TypeScript]
- [Nodemon]
- [Dotenv]

---

## Installation du projet

### Cloner le dépôt
```bash
git clone https://github.com/kyliandeffaut/Creation-d-API.git
cd Creation-d-API

Installer les dépendances

npm install

Structure du projet

Creation-d-API/
├── src/
│   ├── controllers/
│   │   └── user.controller.ts
│   ├── routes/
│   │   └── user.routes.ts
│   └── index.ts
├── .env
├── nodemon.json
├── package.json
├── tsconfig.json
└── README.md

Lancement de l’API
En mode développement

npm run dev

Serveur accessible sur :
👉 http://localhost:4000

En mode production

Compiler le projet :
npm run build

Lancer le serveur compilé :
npm start

Routes disponibles
GET /

Vérifie que le serveur fonctionne.
Réponse attendue :
"API Node.js avec TypeScript fonctionne !"

GET /users

Retourne la liste des utilisateurs enregistrés (stockés en mémoire).

Exemple de réponse :
{
  "users": [
    { "name": "Alice", "email": "alice@example.com" }
  ]
}

POST /users

Ajoute un nouvel utilisateur.

Requête :
curl -X POST http://localhost:4000/users \
-H "Content-Type: application/json" \
-d '{"name":"Alice","email":"alice@example.com"}'

Réponse attendue :
{
  "message": "Utilisateur Alice ajouté avec succès !",
  "email": "alice@example.com"
}
