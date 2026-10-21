# ✨ Mon Espace

Un site web immersif offert en cadeau : un voyage féerique qui raconte votre histoire d’amour
(scrollytelling + expérience immersive + roman visuel interactif).

## 📁 Fichiers

```
lili-monde-magique/
├── index.html          ← le site complet (à ouvrir dans un navigateur)
├── README.md           ← ce guide
└── images/             ← les décors peints des chapitres
    ├── etoiles.jpg     (Chapitre I — La Nuit Étoilée)
    ├── foret.jpg       (Chapitre II — La Forêt Enchantée)
    ├── ocean.jpg       (Chapitre III — L’Océan des Rêves)
    └── jardin.jpg      (Le Jardin Céleste — la lettre finale)
```

## 💌 Personnaliser le site (2 minutes)

Tout le contenu se trouve dans le bloc `CONFIG` en haut du `<script>` dans `index.html` :

1. **`author`** → remplace `"[Ton prénom]"` par ton vrai prénom (signature finale).
2. **`startDate`** → la date de votre rencontre (ex : `"2023-06-21T18:30:00"`).
   Le compteur d’amour s’ajustera automatiquement.
3. **`chapters`** → réécris les 4 chapitres avec vos vrais souvenirs (label, title, text).
4. **`letter`** → ta lettre d’amour qui s’écrit à la fin du voyage.
5. **`memories`** → les 6 cartes « trésors » (icône, titre, texte).
6. **`choices`** → les 3 choix interactifs du roman visuel.
7. **`scratch`** → le message secret de la carte à gratter (ex : un bon pour un week-end).

💡 Astuce : pour ajouter **vos photos**, remplace l’image d’un chapitre dans `images/`
(avec le même nom de fichier), ou ajoute une carte `<img>` dans le Bento.

## 🎵 La musique

Le site génère une **mélodie douce automatique** (Web Audio, aucun fichier nécessaire).
Le bouton 🎵 en haut à droite permet de couper/remettre le son.
Pour utiliser votre propre chanson, ajoute dans `<body>` :

```html
<audio id="ma-chanson" loop src="images/notre-chanson.mp3"></audio>
```

puis dans le script, remplacez `startPad()` par `document.getElementById('ma-chanson').play()`.

## 🚀 Mettre le site en ligne (gratuit)

### Option 1 — Netlify Drop (le plus simple, 30 secondes)
1. Va sur https://app.netlify.com/drop
2. Glisse-dépose le dossier `lili-monde-magique`
3. Ton site est en ligne ! (adresse du type `magnifique-etoile.netlify.app`)

### Option 2 — GitHub Pages
1. Crée un compte sur https://github.com et un nouveau dépôt public
2. Ajoute les fichiers (dont `index.html` à la racine)
3. Dans **Settings → Pages**, choisis la branche `main`
4. Ton site est sur `ton-pseudo.github.io/nom-du-depot`

### Option 3 — Vercel
1. Va sur https://vercel.com et importe le dossier
2. Un clic sur « Deploy » et c’est en ligne

## 🌍 Nom de domaine (optionnel, ~5-10 €/an)

Pour la touche finale, réserve un nom personnalisé chez **Gandi**, **o2switch** ou **Hostinger** :
- `je-taime-lili.fr`
- `notrehistoire-lili.com`
- `pour-ma-lili.love`

Puis lie-le à ton hébergement (Netlify/Vercel proposent un guide « custom domain »).

---

Fait avec ♥ — bonne surprise à toi !
