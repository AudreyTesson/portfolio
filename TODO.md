# TODO - Portfolio Astro

## Avant mise en ligne

### Contenu à personnaliser
- [ ] Remplacer `contact@aurelie.dev` par la vraie adresse email
- [ ] Ajouter les vrais liens LinkedIn, GitHub, Twitter dans le footer
- [ ] Vérifier/modifier les URLs GitHub des projets (logidoc-ai, saas-boilerplate, etc.)
- [ ] Ajouter de vraies screenshots dans les pages projets (remplacer les placeholders)

### Formulaire de contact
- [ ] Connecter le formulaire à un service (options) :
  - Formspree (gratuit, simple)
  - Netlify Forms (si déployé sur Netlify)
  - API custom (Symfony)
  - EmailJS

### SEO & Analytics
- [ ] Ajouter Google Analytics ou Plausible
- [ ] Créer `robots.txt` dans `/public`
- [ ] Créer `sitemap.xml` (ou utiliser `@astrojs/sitemap`)
- [ ] Ajouter Open Graph meta tags pour partage réseaux sociaux
- [ ] Vérifier les meta descriptions de chaque page

### Assets
- [ ] Remplacer le favicon par un vrai logo
- [ ] Ajouter une photo de profil (page About)
- [ ] Ajouter des screenshots réels des projets
- [ ] Optimiser les images (format WebP)

---

## Déploiement

### Option 1 : Vercel (recommandé)
```bash
# 1. Push sur GitHub
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/TON-USERNAME/portfolio.git
git push -u origin main

# 2. Connecter à Vercel
# - Aller sur vercel.com
# - Import Git Repository
# - Sélectionner le repo
# - Deploy (config auto-détectée)
```

### Option 2 : Netlify
```bash
# Même process, importer depuis GitHub sur netlify.com
```

### Option 3 : Déploiement manuel
```bash
npm run build
# Upload le dossier /dist sur ton hébergeur
```

---

## Améliorations futures (optionnel)

### Fonctionnalités
- [ ] Mode sombre / clair toggle
- [ ] Animations au scroll (Intersection Observer)
- [ ] Page 404 custom
- [ ] Blog avec Astro Content Collections
- [ ] Témoignages clients (quand tu en auras)
- [ ] Section "Certifications" si pertinent

### Performance
- [ ] Lazy loading images
- [ ] Preload fonts critiques
- [ ] Minifier le CSS custom

### Accessibilité
- [ ] Vérifier les contrastes (WCAG AA)
- [ ] Ajouter `aria-labels` où nécessaire
- [ ] Tester navigation clavier

---

## Notes

- Le projet utilise **Tailwind CSS v4** (nouvelle syntaxe `@theme`)
- Les couleurs custom sont définies dans `src/styles/global.css`
- Le layout principal est dans `src/layouts/Layout.astro`
- Build testé : 11 pages en 1.6s
