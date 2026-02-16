Déploiement sur GitHub Pages
Étape 1 : Créer le repository GitHub
Connecte-toi sur github.com

Clique sur le bouton "New" ou "+" en haut à droite → "New repository"

Nomme ton repository : kreol-trend-974 (ou le nom de ton choix)

Coche "Public" (obligatoire pour GitHub Pages gratuit)

Coche "Add a README file"

Clique sur "Create repository"

Étape 2 : Organiser les fichiers
Crée cette structure de dossiers sur ton ordinateur :

text
kreol-trend-974/
├── index.html
├── images/
│   ├── KREOLTREND-974.jpg
│   └── fatigue-magasinier.jpg
└── videos/
    └── KREOL-TREND_974___Mission_Super-Samedi.mp4
⚠️ IMPORTANT pour la vidéo :

GitHub limite les fichiers à 25 MB par upload direct

Ta vidéo fait 11 MB, donc ça passe ! ✅

Si elle était trop lourde, il faudrait utiliser Git LFS ou héberger ailleurs

Étape 3 : Uploader les fichiers sur GitHub
Option A : Via l'interface web (plus simple)

Sur ton repository GitHub, clique sur "Add file" → "Upload files"

Glisse-dépose index.html directement à la racine

Clique sur "Commit changes"

Clique sur "Add file" → "Create new file"

Dans le nom, tape images/temp.txt (pour créer le dossier)

Ajoute n'importe quel texte, puis "Commit new file"

Va dans le dossier images/ et clique "Add file" → "Upload files"

Glisse-dépose tes 2 images JPG

Répète pour créer le dossier videos/ et uploader la vidéo MP4

Option B : Via Git en ligne de commande

bash
# Clone le repository
git clone https://github.com/TON-USERNAME/kreol-trend-974.git
cd kreol-trend-974

# Copie tous tes fichiers dans ce dossier (respecte la structure)

# Ajoute et pousse les fichiers
git add .
git commit -m "Ajout du site KREOL-TREND 974"
git push origin main
Étape 4 : Activer GitHub Pages
Sur ton repository, clique sur "Settings" (en haut à droite)

Dans le menu latéral gauche, clique sur "Pages"

Sous "Source", sélectionne "Deploy from a branch"

Sous "Branch", sélectionne "main" et "/ (root)"

Clique sur "Save"

⏰ Attends 1-5 minutes que GitHub déploie ton site

Étape 5 : Accéder à ton site
Ton site sera accessible à :

text
https://TON-USERNAME.github.io/kreol-trend-974/
Remplace TON-USERNAME par ton nom d'utilisateur GitHub.

📹 Note sur la vidéo
La vidéo est intégrée en HTML5 natif avec :

xml
<video controls poster="./images/KREOLTREND-974.jpg">
    <source src="./videos/KREOL-TREND_974___Mission_Super-Samedi.mp4" type="video/mp4">
</video>
Avantages :

✅ Lecture directe dans le navigateur

✅ Contrôles natifs (play, pause, volume)

✅ Poster (image de prévisualisation) avant lecture

✅ Pas de dépendance externe (YouTube, Vimeo, etc.)

Si la vidéo ne charge pas :

Vérifie que le chemin est correct : ./videos/KREOL-TREND_974___Mission_Super-Samedi.mp4

Vérifie que la vidéo est bien uploadée dans le dossier videos/

Ouvre la console développeur (F12) pour voir les erreurs

🎨 Fonctionnalités du site
✨ Design manga interactif avec animations

📹 Vidéo de présentation intégrée

🖼️ Images illustratives (entrepôt + magasinier)

📊 4 missions détaillées avec répartition des rôles

📋 Tableaux de données interactifs (annexes pliables)

📱 Responsive (mobile, tablette, desktop)

🎯 Animations au scroll et au survol

🛠️ Modifications futures
Pour modifier le site :

Clone le repository (si pas déjà fait)

Modifie index.html avec ton éditeur de texte

Teste en local en ouvrant index.html dans un navigateur

Pousse les changements :

bash
git add index.html
git commit -m "Description des modifications"
git push origin main
GitHub Pages se mettra à jour automatiquement en 1-5 minutes.

📧 Contact
Formateur : Sylvain
Email : formateur1.successformation@gmail.com

Bon courage aux apprenants pour le Super-Samedi ! 🔥
