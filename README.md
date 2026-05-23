# 🧊 Mon Frigo — PWA

Application mobile de gestion de frigo et placards avec scan de codes-barres et synchronisation en temps réel entre plusieurs téléphones.

---

## Activer la synchronisation Firebase (partage entre téléphones)

### Étape 1 — Créer un projet Firebase (gratuit)
1. Va sur **https://console.firebase.google.com**
2. Clique **"Créer un projet"**
3. Nomme-le `mon-frigo` (ou ce que tu veux)
4. Désactive Google Analytics (pas nécessaire)
5. Clique **"Créer le projet"**

### Étape 2 — Activer Realtime Database
1. Dans le menu gauche : **Build → Realtime Database**
2. Clique **"Créer une base de données"**
3. Choisis la région **Europe (belgium)** ou **europe-west1**
4. Mode : choisis **"Commencer en mode test"** (tu pourras sécuriser plus tard)
5. Clique **Activer**

### Étape 3 — Récupérer tes identifiants
1. Clique sur la roue ⚙️ à côté de "Vue d'ensemble du projet" → **Paramètres du projet**
2. Fais défiler jusqu'à **"Vos applications"**
3. Clique sur l'icône **`</>`** (Web)
4. Nomme l'app `frigo-pwa`, clique **Enregistrer l'application**
5. Tu verras un bloc `firebaseConfig` avec :
   - `apiKey: "AIzaSy..."` → c'est ta **Clé API**
   - `projectId: "mon-frigo-xxxxx"` → c'est ton **ID du projet**

### Étape 4 — Connecter dans l'app
1. Ouvre l'app sur ton téléphone
2. Dans l'onglet Scanner, un encadré vert apparaît
3. Colle la **Clé API** et l'**ID du projet**
4. Appuie sur **"Connecter Firebase"**
5. Fais la même chose sur le téléphone de Ninie

✅ Les deux téléphones sont maintenant synchronisés en temps réel !

---

## Fonctionnalités

- 📷 Scan caméra en temps réel (codes-barres 1D et QR)
- 🔍 Identification automatique via Open Food Facts
- 🧊 Gestion Frigo / Congélateur / Placard + emplacements personnalisés
- ✏️ Modification des articles (emplacement, DLC, quantité)
- ⚡ Synchronisation temps réel via Firebase (plusieurs téléphones)
- ⚠️ Alertes DLC
- 📊 Tableau de bord
- 📱 Installable sur iPhone et Android (PWA)
