# LUMIÈRE — Responsive Store Landing Page

## 📁 Fichiers
- `index.html` — structure de la page (header, product section, footer)
- `styles.css` — styles personnalisés complémentaires à Tailwind

## 🛠️ Stack technique
- **HTML5 sémantique**
- **Tailwind CSS** (CDN) — framework choisi pour la responsivité (bonus de l'énoncé)
- **CSS personnalisé** — pour les effets non couverts par les utilitaires
- **JavaScript léger** (~10 lignes) — menu hamburger mobile fonctionnel

## 🎨 Design choices

### Palette
Palette **neutre et chaleureuse** (`neutral-50` → `neutral-900`) inspirée du
minimalisme scandinave. Elle met les produits en valeur sans distraire.

### Typographie
Police système (`system-ui`) + poids **light** (300) pour un rendu éditorial.
L'italique est utilisé ponctuellement sur le mot "âme" du hero.

### Layout
- **Header sticky** avec `backdrop-blur` → navigation accessible en permanence
- **Hero centré** sur max-width 720px pour une lecture confortable
- **Grille produits** : `grid-cols-1 → sm:grid-cols-2 → lg:grid-cols-4`
- **Footer** en 4 colonnes sur desktop, empilé sur mobile

### Interactions
- Cartes produits : `translateY(-6px)` + ombre douce au survol
- Boutons "Shop Now" noirs arrondis avec transition
- Menu mobile : ouverture/fermeture JS + fermeture auto au clic sur un lien
- Smooth scrolling sur les ancres

### Accessibilité
- `aria-expanded` + `aria-controls` sur le bouton hamburger
- Focus visible personnalisé
- `sr-only` pour les labels non visuels

## 📱 Responsive (breakpoints testés)

| Largeur | Grille produits | Navigation |
|---------|-----------------|------------|
| 320px   | 1 colonne       | hamburger  |
| 640px   | 2 colonnes      | hamburger  |
| 768px   | 2 colonnes      | nav horizontale |
| 1024px  | 4 colonnes      | nav horizontale |
| 1440px  | 4 colonnes      | nav horizontale |

## 📸 Comment générer les screenshots

1. Ouvrir `index.html` dans Chrome/Firefox
2. `F12` → `Ctrl+Shift+M` (mode responsive)
3. Desktop : largeur 1440px → `Ctrl+Shift+P` → "Capture full size screenshot"
4. Mobile : iPhone 12 Pro (390px) → même commande
5. Enregistrer comme `screenshot-desktop.png` et `screenshot-mobile.png`

## ✅ Exigences couvertes
- [x] Header, product section, footer
- [x] Placeholder content
- [x] Nav menu avec ancres vers sections
- [x] 4 cartes produits (image, nom, description, "Shop Now")
- [x] Design responsive (mobile + desktop)
- [x] Media queries (Tailwind + CSS custom)
- [x] Framework CSS : **Tailwind** ✅ (bonus)
- [x] Menu mobile fonctionnel
- [x] Code commenté et propre