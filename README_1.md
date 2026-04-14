# Arkade Group — Site Web Officiel

Site vitrine pour **Arkade Group**, un groupe ivoirien présent dans deux secteurs : l'événementiel haut de gamme (*Arkade Event*) et l'immobilier & décoration d'intérieur (*Arkade Constructing*).

---

## Aperçu

Le site est une **page unique** (one-page) en HTML/CSS/JS pur, sans dépendances externes ni framework. Il présente les deux divisions du groupe, un catalogue de produits et services avec tarifs, des témoignages clients et un formulaire de contact via WhatsApp.

---

## Structure du projet

```
arkade-group/
├── index.html                  # Fichier principal (page unique)
├── arkad-removebg-preview.png  # Logo Arkade Group
│
├── — Images Arkade Event —
├── decorevent.jpg              # Visuel panneau Brand Split (Event)
├── cleanroom.jpeg              # Galerie — Couverture de chambre
├── dragée.jpeg                 # Galerie — Paniers de dragées
├── serviette.jpeg              # Galerie — Serviettes décoratives
├── imagesdedo.jpg              # Catalogue — Pack Essentiel
├── decoeclairé.jpg             # Catalogue — Pack Prestige
├── decoprenium.avif            # Catalogue — Pack Royal
├── suitelove.jpg               # Catalogue — Suite Romantique
├── suiteking.jpg               # Catalogue — Suite Royale
├── s-tableperso.jpg            # Catalogue — Serviettes & Nappage
├── tradi.jpg                   # Catalogue — Panier Classique
├── dragéebte.jpg               # Catalogue — Panier Prestige
├── draemariage.jpg             # Catalogue — Pack Cérémonie
│
└── — Images Arkade Constructing —
    ├── immo&decor.jpg          # Visuel panneau Brand Split (Constructing)
    ├── agencer-lespace-interieur.jpg  # Section Constructing
    ├── consielimmo.jpg         # Catalogue — Conseil Immobilier
    ├── desinterne.jpg          # Catalogue — Décoration d'Intérieur
    └── homestating.jpg         # Catalogue — Home Staging
```

---

## Sections de la page

| Section | Ancre | Description |
|---|---|---|
| Navigation | — | Fixe au scroll, responsive avec menu hamburger |
| Hero | `#home` | Accroche principale avec deux CTA |
| Brand Split | — | Présentation des deux divisions en split-screen |
| Arkade Event | `#event` | Services événementiels et statistiques |
| Galerie | `#products` | Aperçu des créations (3 visuels) |
| Catalogue | `#catalogue` | Produits et tarifs par onglet (4 catégories) |
| Arkade Constructing | `#construct` | Services immobiliers et décoration |
| Témoignages | — | Carrousel de clients (défilement automatique) |
| Notre Approche | `#process` | Processus en 4 étapes |
| Contact | `#contact` | CTA final avec email et WhatsApp |
| Footer | — | Liens, réseaux sociaux, informations légales |

---

## Technologies

- **HTML5** — structure sémantique
- **CSS3** — variables CSS, Grid, Flexbox, animations, `@keyframes`
- **JavaScript vanilla** — curseur personnalisé, scroll-reveal, onglets catalogue, menu mobile
- **Google Fonts** — `Cormorant Garamond` (titres) + `Jost` (corps de texte)

Aucune dépendance npm, aucun bundler requis.

---

## Déploiement

Le site est statique et peut être hébergé sur n'importe quelle plateforme :

```bash
# Option 1 — Ouvrir localement
open index.html

# Option 2 — Serveur local simple (Python)
python3 -m http.server 8000

# Option 3 — Déploiement GitHub Pages, Netlify, Vercel...
# Déposer tous les fichiers à la racine du dépôt/répertoire public
```

> **Important** : toutes les images doivent être placées dans le même dossier que `index.html` car les chemins sont relatifs à la racine.

---

## Personnalisation

### Couleurs principales (variables CSS dans `:root`)

| Variable | Valeur | Usage |
|---|---|---|
| `--bottle-green` | `#1a3a2a` | Fond principal vert |
| `--gold` | `#c9a84c` | Accents dorés |
| `--black` | `#0a0a0a` | Fond sombre |
| `--white` | `#f5f0e8` | Texte clair |

### Modifier les prix du catalogue

Les prix sont dans les blocs `.cat-price-value` de la section `#catalogue`. Chaque carte produit contient aussi un lien WhatsApp pré-rempli à adapter :

```html
<a href="https://wa.me/2250749110087?text=Votre%20message" ...>
```

### Modifier le numéro WhatsApp

Remplacer toutes les occurrences de `2250749110087` par votre numéro au format international (sans `+`).

### Modifier l'adresse email

Remplacer `contact@arkadegroup.ci` dans le CTA de contact.

---

## Contact & Crédits

- **Entreprise** : Arkade Group — Abidjan, Côte d'Ivoire
- **Téléphone** : +225 07 49 11 00 87
- **Développement** : [kode-ldev.io](https://christoth-king.github.io/Kode-ldev/)
- **Réseaux** : [Facebook](https://www.facebook.com/share/p/1aXMrE1wCv/) · WhatsApp

---

© 2025 Arkade Group · Tous droits réservés
