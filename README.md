# 🧊 Mon Frigo — PWA

Application mobile de gestion de frigo et placards avec scan de codes-barres.

## Fonctionnalités

- 📷 **Scan caméra** en temps réel (codes-barres 1D et QR)
- 🔍 **Identification automatique** via Open Food Facts (millions de produits)
- 🧊 Gestion **Frigo / Congélateur / Placard / Corbeille**
- ⚠️ **Alertes DLC** (produits expirant bientôt)
- 📊 **Tableau de bord** avec statistiques
- 📱 **Installable** sur iPhone et Android (PWA)
- ✈️ Fonctionne **hors-ligne** (données en cache)

---

## Déploiement sur GitHub Pages (gratuit, 5 minutes)

### Étape 1 — Créer un compte GitHub
→ https://github.com/signup (gratuit)

### Étape 2 — Créer un nouveau dépôt
1. Cliquez sur **"New repository"**
2. Nommez-le `frigo-app` (ou ce que vous voulez)
3. Cochez **"Public"**
4. Cliquez **"Create repository"**

### Étape 3 — Uploader les fichiers
1. Dans votre nouveau dépôt, cliquez **"uploading an existing file"**
2. Glissez-déposez tous les fichiers du dossier `frigo-app/` :
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - le dossier `icons/` avec `icon-192.png` et `icon-512.png`
3. Cliquez **"Commit changes"**

### Étape 4 — Activer GitHub Pages
1. Allez dans **Settings** → **Pages**
2. Sous "Source", choisissez **"Deploy from a branch"**
3. Choisissez la branche **main** et le dossier **/ (root)**
4. Cliquez **Save**

### Étape 5 — Accéder à votre app
Votre app sera disponible à :
```
https://VOTRE_USERNAME.github.io/frigo-app/
```
(remplacez VOTRE_USERNAME par votre nom d'utilisateur GitHub)

---

## Installer l'app sur votre téléphone

### Sur iPhone (Safari obligatoire)
1. Ouvrez l'URL dans **Safari**
2. Appuyez sur le bouton **Partager** (carré avec flèche)
3. Choisissez **"Sur l'écran d'accueil"**
4. Appuyez **Ajouter**

### Sur Android (Chrome)
1. Ouvrez l'URL dans **Chrome**
2. Un bandeau "Installer l'application" apparaît automatiquement
3. Sinon : menu ⋮ → **"Ajouter à l'écran d'accueil"**

---

## Notes techniques

- Les données sont stockées localement dans le navigateur (localStorage)
- L'identification des produits utilise l'API Open Food Facts (open source, gratuite)
- La caméra nécessite HTTPS (fourni automatiquement par GitHub Pages)
- Compatible iOS 14.5+ et Android 8+
