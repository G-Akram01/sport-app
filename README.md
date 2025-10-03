# 🏋️‍♂️ Test application Club de Sport  

Application web pour **la gestion des cours sportifs et des réservations**.  
Ce projet a été développé dans le cadre d’un exercice Agile (Scrum) avec un MVP (Itération 1) permettant :  
- Inscription / Connexion (utilisateur & coach)  
- Création de créneaux par les coachs  
- Consultation du planning des cours  
- Réservation de séances par les utilisateurs  

---

## 🚀 Getting Started  

### 📦 Prérequis  
- [Node.js](https://nodejs.org/) (>= 16.x)  
- [npm](https://www.npmjs.com/) ou [yarn](https://yarnpkg.com/)  
- (optionnel) [PostgreSQL](https://www.postgresql.org/) si vous voulez persister les données côté backend  

---

### ▶️ Lancer le projet en mode développement  

```bash
npm install
npm start
```
Ouvrir http://localhost:3000 dans votre navigateur.
L’app se rechargera automatiquement si vous modifiez le code.

### 🧪 Lancer les tests
```bash
npm test
```

Les tests s’exécutent en mode interactif (utile pour vérifier signup, login, réservation).

### 🏗️ Construire l’application pour la production
npm run build


Les fichiers seront générés dans le dossier build/

Code optimisé et minifié

Prêt à être déployé (Netlify, Vercel, Heroku, etc.)

### 📚 Fonctionnalités du MVP (Itération 1)

#### ✅ Utilisateur

Inscription (Signup)

Connexion sécurisée (Login JWT simulé)

Consulter le planning des cours

Réserver une séance si places disponibles

Voir ses réservations

#### ✅ Coach

Connexion (accès à l’espace Coach)

Créer / Supprimer des créneaux de cours

Voir l’état de remplissage de ses cours

### 📂 Structure du projet
```
/src
 ├── App.js        # Composant principal (routing + navigation)
 ├── components/   # Composants réutilisables (formulaires, cartes, boutons…)
 ├── pages/        # Pages principales (Login, Signup, Planning, Coach…)
 ├── services/     # (Optionnel) appels API backend
```
### 🔗 Backend (API REST) – MVP

Le backend est minimal et fournit :
```
POST /auth/signup – créer un compte

POST /auth/login – se connecter

POST /class-slots – créer un créneau (coach)

GET /class-slots – consulter le planning

POST /bookings – réserver un cours

GET /bookings/me – mes réservations
```
