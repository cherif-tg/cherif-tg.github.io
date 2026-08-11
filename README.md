# Portfolio — TENGA Chérif Abdel Azize

Portfolio professionnel de Data Scientist & AI Engineer.

## 🚀 Démarrer

```bash
# Installer les dépendances
npm install

# Lancer en développement
npm run dev

# Builder pour la production
npm run build
```

Le build génère un site statique dans `out/`, déployable sur n'importe quel hébergeur statique (Vercel, Netlify, GitHub Pages, etc.).

## 📁 Structure

```
src/
├── app/
│   ├── layout.tsx       # Layout global (SEO, fonts)
│   ├── page.tsx         # Page principale (one-page)
│   └── globals.css      # Styles globaux + Tailwind
├── components/
│   ├── Navbar.tsx       # Navigation fixe
│   ├── Hero.tsx         # Hero + animation canvas
│   ├── About.tsx        # Bio, formation, contact
│   ├── Skills.tsx       # Grille de compétences
│   ├── Projects.tsx     # Projets détaillés
│   ├── Certifications.tsx
│   ├── Contact.tsx      # Liens + stage
│   └── ParticleBackground.tsx  # Animation réseau de neurones
├── lib/
│   └── data.ts          # TOUTES les données du site
└── public/
    ├── cv.pdf
    └── certif-ai-engineer.pdf
```

## ✏️ Comment modifier

### Modifier le contenu
**Un seul fichier à éditer :** `src/lib/data.ts`

- **Infos perso :** objet `personalInfo` (nom, titre, email, bio)
- **Formation :** tableau `education`
- **Compétences :** tableau `skills` (catégories + items)
- **Projets :** tableau `projects` — ajouter un projet = ajouter un objet
- **Certifications :** tableau `certifications`
- **Liens sociaux :** objet `socialLinks`

### Modifier le design
- **Couleurs :** `tailwind.config.js` → section `colors`
- **Typographie :** `src/app/globals.css` → `@import url(...)` + `tailwind.config.js` → `fontFamily`
- **Styles globaux :** `src/app/globals.css`

### Ajouter un projet
1. Ouvrir `src/lib/data.ts`
2. Ajouter un objet dans le tableau `projects` :
```ts
{
  slug: 'mon-nouveau-projet',
  title: 'Titre du projet',
  subtitle: 'Contexte • Année',
  description: 'Description courte...',
  highlights: ['Point clé 1', 'Point clé 2'],
  stack: ['Python', 'PyTorch', ...],
}
```
3. Rebuilder : `npm run build`

### Déployer
```bash
npm run build
# → Le dossier out/ contient le site statique
# Déployer out/ sur Vercel, Netlify, ou GitHub Pages
```

## 🎨 Design System

- **Philosophie :** Takram — soft tech, élégance japonaise
- **Palette :** Crème (#FAF7F2), tons chauds, accent vert muted (#5B8C5A)
- **Typographie :** Inter (corps) + DM Serif Display (titres)
- **Animation :** Particules canvas interactives (réseau de neurones)

## ✅ Qualité

- [x] Responsive (mobile + desktop)
- [x] Navigation fluide (scroll smooth)
- [x] Animations CSS (fade-in, float)
- [x] Canvas interactif (particules connectées)
- [x] Accessibilité (ARIA labels, contraste)
- [x] SEO (meta tags, Open Graph)
- [x] Export statique (déploiement universel)
