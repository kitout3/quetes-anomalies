# Quêtes d'Anomalies - Multijoueur Firebase

Jeu de plateau multijoueur en temps réel avec synchronisation Firebase.

## 🚀 Installation

### 1. Créer un projet Firebase

1. Allez sur [console.firebase.google.com](https://console.firebase.google.com)
2. Créez un nouveau projet
3. Activez **Authentication** > **Anonymous** (Sign-in method)
4. Créez une **Realtime Database** (région europe-west1, mode test)
5. Copiez la configuration Firebase

### 2. Configurer le jeu

Ouvrez `index.html` et remplacez les valeurs de `firebaseConfig` (vers ligne 25):

```javascript
const firebaseConfig = {
  apiKey: "VOTRE_API_KEY",
  authDomain: "VOTRE_PROJECT.firebaseapp.com",
  databaseURL: "https://VOTRE_PROJECT-default-rtdb.europe-west1.firebasedatabase.app",
  projectId: "VOTRE_PROJECT",
  storageBucket: "VOTRE_PROJECT.appspot.com",
  messagingSenderId: "VOTRE_SENDER_ID",
  appId: "VOTRE_APP_ID"
};
```

### 3. Déployer sur GitHub Pages

1. Créez un repository GitHub
2. Uploadez les fichiers (glisser-déposer)
3. Settings → Pages → Source: main → Save
4. Attendez 2 minutes → Votre jeu est en ligne !

## 🎮 Fonctionnalités

- **Multijoueur temps réel** (2-6 joueurs)
- **Code de partie** (6 caractères)
- **6 personnages** avec capacités uniques
- **Allocation de stats** (-2, -1, 0, 0, +1, +2)
- **7 onglets de jeu**:
  - 🎴 Tirages (Anomalies + Quêtes)
  - 🎲 Dé (Déplacement + Attaque)
  - ⚔️ Attaque (Territoires + Boss)
  - 🎯 Objectif (Quêtes + Ressources)
  - 🔄 Échange (Conversion + Joueurs)
  - 👤 Personnage (PV + Stats + États)
  - 🏆 PDV (Score + Classement)

## 📱 Installation PWA

- **iPhone**: Safari → Partager → Sur l'écran d'accueil
- **Android**: Chrome → Menu → Installer l'application

## 🎯 Règles rapides

- **Objectif**: Atteindre 10 PDV × nombre de joueurs
- **Tour**: Tirages → Actions → Fin de tour
- **PDV**: Territoires, Boss, Quêtes, Objectifs, Passage Départ

## 📁 Fichiers

- `index.html` - Application complète
- `manifest.json` - Configuration PWA
- `README.md` - Documentation
