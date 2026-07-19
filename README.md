# Site personnel — Marc Garnier

Site vitrine statique (HTML / CSS / JS, aucune dépendance à installer).

## Structure

- `index.html` — accueil : hero, statistiques, à propos, travaux en cours, contact
- `thesis.html` — page détaillée du projet de thèse (timeline, corpus, pipeline, schéma d'annotation)
- `projects.html` — projets en cours (un gabarit commenté explique comment ajouter une carte)
- `cv.html` — expériences, formation, certifications, outils
- `css/style.css` — tout le style (palette et typographie définies dans `:root` en haut du fichier)
- `js/main.js` — menu mobile, animations d'apparition, année du footer

## Personnalisation rapide

- **Photo** : placez votre portrait dans `assets/` (ex. `assets/portrait.jpg`), puis dans
  `index.html`, remplacez le bloc `portrait-placeholder` par
  `<img class="portrait" src="assets/portrait.jpg" alt="Portrait of Marc Garnier">`
  (le commentaire HTML sur place vous montre où).
- **LinkedIn** : dans `index.html`, section contact, remplacez `https://www.linkedin.com/`
  par l'URL de votre profil.
- **Ajouter un projet** : dans `projects.html`, dupliquez le bloc commenté
  « HOW TO ADD A PROJECT ».
- **Couleurs** : modifiez les variables dans `:root` au début de `css/style.css`.

## Déploiement sur GitHub Pages

1. Créez un dépôt GitHub nommé `VOTRE-USERNAME.github.io` (ou n'importe quel nom).
2. Dans ce dossier :
   ```bash
   git init
   git add .
   git commit -m "Site personnel"
   git branch -M main
   git remote add origin https://github.com/VOTRE-USERNAME/VOTRE-DEPOT.git
   git push -u origin main
   ```
3. Sur GitHub : **Settings → Pages → Source : Deploy from a branch → main / (root) → Save**.
4. Le site sera en ligne quelques minutes plus tard à
   `https://VOTRE-USERNAME.github.io/` (ou `/VOTRE-DEPOT/` si le dépôt porte un autre nom).

## Aperçu local

Ouvrez simplement `index.html` dans un navigateur, ou lancez :

```bash
python3 -m http.server 8000
```

puis visitez <http://localhost:8000>.
