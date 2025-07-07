# expense_tracker_with_budgeting


# 📱💸 Expense Tracker with Budgeting

## 🌟 Description

**Expense Tracker with Budgeting** est une application mobile développée avec **Flutter**, accompagnée d’un backend **Node.js/Express/MongoDB**, permettant aux utilisateurs de :

- Enregistrer leurs dépenses
- Définir des budgets par catégorie
- Visualiser leurs habitudes de consommation via des graphiques
- Recevoir des alertes en cas de dépassement de budget

> Projet réalisé dans le cadre des modules _Mobile Development_ et _Web Services with REST API Development_.

---

## 📦 Fonctionnalités

### 👤 Utilisateurs
- Authentification sécurisée (JWT)
- Inscription / Connexion

### 💸 Dépenses
- Ajouter / Modifier / Supprimer des dépenses
- Vue par catégorie, date, ou montant

### 📊 Budgets
- Définir des limites par catégorie
- Suivi mensuel ou hebdomadaire
- Alertes intelligentes

### 📈 Visualisation
- Graphiques (camembert, barres)
- Résumés mensuels/hebdomadaires
- Historique des dépenses

### ⚙️ Options supplémentaires (facultatif)
- Export en CSV ou PDF
- Sélection de devise ou langue

---

## 🧰 Technologies

- **Flutter** (mobile)
- **Node.js** + **Express** (backend)
- **MongoDB** + Mongoose (base de données)
- JWT, bcrypt, Provider, Charts, etc.

---

## 📁 Structure du Projet

```

expense-tracker/
├── mobile/        # App Flutter
├── backend/       # API Node.js/Express
└── docs/          # Captures d’écran, export, slides

````

---

## 🚀 Installation & Lancement

### 1. Cloner le projet

```bash
git clone https://github.com/votre-utilisateur/expense-tracker.git
cd expense-tracker
````

### 2. Lancer le Backend

```bash
cd backend
npm install
touch .env
```

Créer un fichier `.env` :

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/expense-tracker
JWT_SECRET=your_jwt_secret
```

Lancer le serveur :

```bash
npm start
```

### 3. Lancer l'application Flutter

```bash
cd mobile
flutter pub get
flutter run
```

---

## 🔌 API Endpoints Principaux

| Méthode | Endpoint             | Description              |
| ------- | -------------------- | ------------------------ |
| POST    | /api/auth/register   | Inscription              |
| POST    | /api/auth/login      | Connexion                |
| GET     | /api/expenses        | Lister les dépenses      |
| POST    | /api/expenses        | Ajouter une dépense      |
| PUT     | /api/expenses/\:id   | Modifier une dépense     |
| DELETE  | /api/expenses/\:id   | Supprimer une dépense    |
| GET     | /api/budgets         | Liste des budgets        |
| POST    | /api/budgets         | Créer un budget          |
| GET     | /api/reports/summary | Résumé analytique        |
| GET     | /api/reports/export  | Exporter CSV/PDF *(opt)* |

👉 Collection **Postman** disponible dans `/docs/Postman_collection.json`.

---

## 🧪 Exemples de Données

### Utilisateur

```json
{
  "name": "Alice",
  "email": "alice@example.com",
  "password": "$2a$10$..."
}
```

### Dépense

```json
{
  "userId": "ObjectId",
  "amount": 75.50,
  "category": "transport",
  "note": "Bus mensuel",
  "date": "2025-07-01T10:00:00Z"
}
```

### Budget

```json
{
  "userId": "ObjectId",
  "category": "transport",
  "limit": 150,
  "period": "monthly"
}
```

---

## 📸 Captures d'écran

| Formulaire Dépense     | Tableau de Bord                  | Alerte                   |
| ---------------------- | -------------------------------- | ------------------------ |
| ![Form](docs/form.png) | ![Dashboard](docs/dashboard.png) | ![Alert](docs/alert.png) |

---

## 👥 Équipe

| Nom                 | Rôle                            |
| ------------------- | ------------------------------- |
| Jeannine Thiombiano | Développement Flutter & Backend |
|Kabore Pauline       |Développement Flutter & Backend   |
Ziba Luc                
---

## 📖 Présentation

* 🎥 `demo.mp4` – Démonstration de l'application
* 🖼️ `slides.pdf` – Présentation synthétique du projet

> Tous les fichiers sont disponibles dans `/presentation`.

---

## 📄 Licence

Projet open-source à usage éducatif uniquement.
© 2025 - Tous droits réservés.


