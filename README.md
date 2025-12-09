# Portfolio - Aurélie Tesson

Portfolio personnel développé avec Astro + Tailwind CSS.

## Stack

- **Astro** - Framework SSG ultra-performant
- **Tailwind CSS v4** - Styling utilitaire

## Développement

```bash
# Installer les dépendances
npm install

# Lancer le serveur de développement
npm run dev

# Build pour production
npm run build

# Preview de la build
npm run preview
```

## Déploiement Vercel

```bash
# Déploiement manuel
npx vercel

# Ou connecter le repo GitHub à Vercel pour déploiement automatique
```

## Structure

```
src/
├── layouts/
│   └── Layout.astro      # Layout principal (nav + footer)
├── pages/
│   ├── index.astro       # Homepage
│   ├── about.astro       # À propos
│   ├── services.astro    # Services
│   ├── projets.astro     # Liste des projets
│   ├── contact.astro     # Contact
│   └── projets/          # Pages projets détaillées
│       ├── wms.astro
│       ├── logidoc-ai.astro
│       └── ...
└── styles/
    └── global.css        # Tailwind + custom CSS
```
