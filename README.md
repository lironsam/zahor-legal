# zahor-legal

Pages légales de l'application **Zahor** (politique de confidentialité, conditions d'utilisation).

Hébergé via **GitHub Pages** pour satisfaire les exigences de publication sur Google Play Store et App Store.

## Déploiement (première fois)

### 1. Créer le repo sur GitHub

```bash
cd /Users/lironesamoun/Documents/zahor-legal
git init
git add .
git commit -m "chore: initial privacy policy (FR + EN)"
git branch -M main
```

Puis sur GitHub :
1. https://github.com/new → nom : `zahor-legal` → **Public** → **Create repository**
2. Suivre les instructions pour pousser :

```bash
git remote add origin https://github.com/lironsam/zahor-legal.git
git push -u origin main
```

### 2. Activer GitHub Pages

1. Repo GitHub → **Settings** → **Pages**
2. Source : **Deploy from a branch**
3. Branch : **main** / **root** → **Save**
4. Attendre ~1 min, puis l'URL apparaît en haut de la page :
   ```
   https://lironsam.github.io/zahor-legal/
   ```

### 3. Coller l'URL dans les stores

- **Google Play Console** → ton app → **Policy** → **App content** → **Privacy Policy** → coller l'URL → **Save**
- **App Store Connect** → ton app → **App Privacy** → **Privacy Policy URL** → coller l'URL

## Mise à jour

Edit `index.html` → commit → push. GitHub Pages redéploie automatiquement en ~30 secondes.

N'oublie pas de mettre à jour la date "Dernière mise à jour / Last updated" en haut du document à chaque modification matérielle.

## Contenu

- `index.html` — politique de confidentialité bilingue FR/EN (une seule page, sections ancrées)
- Ajouter plus tard : `terms.html` (CGU) si besoin pour l'App Store
