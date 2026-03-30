# Fromagerie Smine - MERN Stack Application

Une application web complète de gestion de fromagerie développée avec la stack MERN (MongoDB, Express.js, React, Node.js).

## 🚀 Fonctionnalités

### Gestion des Produits
- Ajout, modification et suppression de produits
- Upload d'images multiples (Cloudinary)
- Gestion des quantités, prix d'achat/vente
- Catégorisation des produits

### Gestion des Catégories
- Création et gestion des catégories
- Images représentatives
- Interface intuitive

### Authentification Utilisateur
- Système d'inscription/connexion
- Middleware d'authentification JWT
- Gestion des rôles (Admin/Client)

### Interface Utilisateur
- Design responsive avec Material-UI
- Dashboard administrateur et client
- Gestion des commandes et paiements Stripe

## 🛠️ Technologies Utilisées

### Backend
- **Node.js** & **Express.js** - Serveur API
- **MongoDB** & **Mongoose** - Base de données
- **JWT** - Authentification
- **Cloudinary** - Stockage d'images
- **Stripe** - Paiements
- **Multer** - Upload de fichiers

### Frontend
- **React** - Framework UI
- **Material-UI** - Composants UI
- **React Router** - Navigation
- **Axios** - Requêtes HTTP

## 📁 Structure du Projet

```
projet mern/
├── backend/                 # Serveur Node.js
│   ├── models/             # Schémas MongoDB
│   ├── routes/api/         # Routes API
│   ├── middleware/         # Middleware Express
│   ├── utils/              # Utilitaires (Cloudinary)
│   └── uploads/            # Images locales (fallback)
├── my-frontend-project/     # Application React
│   ├── src/
│   │   ├── components/     # Composants réutilisables
│   │   ├── pages/          # Pages principales
│   │   └── config/         # Configuration API
│   └── public/             # Assets statiques
└── AGENTS.md               # Documentation agents IA
```

## 🚀 Installation et Démarrage

### Prérequis
- Node.js (v16+)
- MongoDB (local ou Atlas)
- Compte Cloudinary (pour les images)
- Compte Stripe (pour les paiements)

### Installation

1. **Cloner le repository**
   ```bash
   git clone https://github.com/Negzaoui948/Froamgerie-Smine.git
   cd projet mern
   ```

2. **Backend**
   ```bash
   cd backend
   npm install
   # Créer .env avec vos clés (voir .env.example)
   npm run start
   ```

3. **Frontend**
   ```bash
   cd ../my-frontend-project
   npm install
   npm start
   ```

### Variables d'environnement

Créer `backend/.env` :
```env
MONGO_URL=mongodb://localhost:27017/fromagerie_db
CLOUDINARY_URL=cloudinary://api_key:api_secret@cloud_name
STRIPE_SECRET_KEY=sk_test_...
PORT=3015
```

## 📡 API Endpoints

### Produits
- `GET /produits` - Liste des produits
- `POST /produits/add` - Ajouter un produit
- `PUT /produits/update/:id` - Modifier un produit
- `DELETE /produits/delete/:id` - Supprimer un produit

### Catégories
- `GET /categories` - Liste des catégories
- `POST /categories/add` - Ajouter une catégorie
- `PUT /categories/update/:id` - Modifier une catégorie
- `DELETE /categories/delete/:id` - Supprimer une catégorie

### Utilisateurs
- `POST /users/register` - Inscription
- `POST /users/login` - Connexion

## 🌐 Déploiement

### Vercel (Recommandé)
1. Connecter le repo GitHub à Vercel
2. Configurer les variables d'environnement
3. Déployer automatiquement

### Configuration Vercel incluse
- `backend/vercel.json` - Configuration backend
- `my-frontend-project/vercel.json` - Configuration frontend

## 🤝 Contribution

1. Fork le projet
2. Créer une branche (`git checkout -b feature/AmazingFeature`)
3. Commit les changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

## 📝 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 👤 Auteur

**Oussama Negzaoui** - [GitHub](https://github.com/Negzaoui948)

## 🙏 Remerciements

- Material-UI pour les composants UI
- Cloudinary pour le stockage d'images
- Stripe pour les paiements
- MongoDB Atlas pour la base de données