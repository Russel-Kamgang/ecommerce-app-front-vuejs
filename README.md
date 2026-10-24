<div align="center">

# E-commerce · Front Vue.js

**Vitrine e-commerce responsive construite avec Vue 3, Vite et TailwindCSS**

![Vue.js](https://img.shields.io/badge/Vue_3-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Iconify](https://img.shields.io/badge/Iconify-1769AA?style=for-the-badge&logo=iconify&logoColor=white)

</div>

---

## Présentation

Interface front-end d'une boutique en ligne, découpée en composants Vue réutilisables. Le projet met l'accent sur une architecture par composants claire, un design responsive mobile-first et un outillage moderne (Vite, Tailwind).

## Sections

| Composant | Contenu |
|-----------|---------|
| `Header.vue` | Barre de navigation |
| `Hero.vue` | Bannière d'accueil |
| `Products.vue` | Catalogue de produits |
| `Categories.vue` | Navigation par catégorie |
| `Offers.vue` | Promotions en cours |
| `About.vue` | Présentation de la boutique |
| `Contact.vue` | Formulaire de contact |
| `Footer.vue` | Pied de page |

## Démarrage

Prérequis : Node.js 20+.

```bash
git clone https://github.com/Russel-Kamgang/ecommerce-app-front-vuejs.git
cd ecommerce-app-front-vuejs

npm install
npm run dev       # http://localhost:5173
npm run build     # build de production dans dist/
npm run preview   # prévisualiser le build
```

## Choix techniques

- **Vue 3 et `<script setup>`** : syntaxe concise de la Composition API
- **Vite** : démarrage instantané et rechargement à chaud
- **TailwindCSS** : styles utilitaires et breakpoints responsive
- **Iconify** (`@iconify/vue`) : accès à plus de 200 000 icônes via `<Icon icon="mdi:home" />`

## Structure

```
src/
├── App.vue           # Assemblage des sections
├── main.js           # Point d'entrée et enregistrement d'Iconify
├── style.css         # Directives Tailwind
└── components/       # Une section = un composant
```

## Feuille de route

- [ ] Panier et gestion d'état avec Pinia
- [ ] Pages produit avec Vue Router
- [ ] Connexion à une API back-end
