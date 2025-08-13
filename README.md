# 🎨 Kit UI - Palette de Couleurs

Un kit UI complet et responsive basé sur votre palette de couleurs personnalisée, prêt à l'emploi pour vos projets web.

## 🌈 Palette de Couleurs

Votre palette comprend 7 couleurs principales :

| Couleur | Code Hex | Nom | Usage |
|---------|----------|-----|-------|
| `#8B5CF6` | Violet vibrant | Primary | Couleur principale, boutons, liens |
| `#6B46C1` | Violet foncé | Primary Dark | Hover states, accents |
| `#93C5FD` | Bleu clair | Secondary | Éléments secondaires, infos |
| `#F8FAFC` | Gris très clair | Gray Light | Arrière-plans secondaires |
| `#FFFFFF` | Blanc | White | Arrière-plans principaux |
| `#374151` | Gris foncé | Gray Dark | Texte principal |
| `#9CA3AF` | Gris moyen | Gray | Texte secondaire, bordures |

## 📁 Structure des Fichiers

```
Monitoring PoC/
├── styles.css          # Kit UI complet avec variables CSS
├── demo.html           # Page de démonstration interactive
└── README.md           # Documentation
```

## 🚀 Utilisation Rapide

### 1. Lier le CSS
```html
<link rel="stylesheet" href="styles.css">
```

### 2. Utiliser les classes utilitaires
```html
<!-- Bouton primary -->
<button class="btn btn-primary">Cliquez-moi</button>

<!-- Carte avec ombre -->
<div class="card">
    <div class="card-header">Titre</div>
    <div class="card-body">Contenu</div>
</div>

<!-- Grille responsive -->
<div class="grid grid-cols-1 md:grid-cols-3 gap-md">
    <div>Colonne 1</div>
    <div>Colonne 2</div>
    <div>Colonne 3</div>
</div>
```

## 🎯 Composants Disponibles

### Boutons
- **Variantes** : `btn-primary`, `btn-secondary`, `btn-outline`, `btn-ghost`
- **Tailles** : `btn-sm`, `btn` (normal), `btn-lg`
- **États** : Hover, focus, active avec animations

### Cartes
- **Structure** : `card-header`, `card-body`, `card-footer`
- **Effets** : Hover avec ombre et animation
- **Responsive** : S'adapte à tous les écrans

### Formulaires
- **Classes** : `form-group`, `form-label`, `form-input`
- **États** : Normal, focus, disabled
- **Validation** : Styles pour succès, erreur, warning

### Alertes
- **Types** : `alert-success`, `alert-warning`, `alert-error`, `alert-info`
- **Design** : Couleurs sémantiques avec transparence

### Badges
- **Variantes** : Primary, secondary, success, warning, error
- **Style** : Ronds avec padding et couleurs appropriées



## 📱 Système Responsive

### Breakpoints
- **Mobile First** : Design optimisé pour mobile
- **SM** : 640px+ (tablettes)
- **MD** : 768px+ (tablettes larges)
- **LG** : 1024px+ (desktop)
- **XL** : 1280px+ (desktop large)

### Classes Responsives
```html
<!-- Caché sur mobile, visible sur desktop -->
<div class="d-none md:d-block">Contenu desktop</div>

<!-- 1 colonne sur mobile, 3 sur desktop -->
<div class="grid grid-cols-1 md:grid-cols-3">
    <!-- Contenu -->
</div>

<!-- Flexbox direction responsive -->
<div class="d-flex flex-col md:flex-row">
    <!-- Contenu -->
</div>
```

## 🎨 Classes Utilitaires

### Couleurs
```css
.bg-primary          /* Fond primary */
.text-primary        /* Texte primary */
.border-primary      /* Bordure primary */
```

### Espacements
```css
.m-md               /* Margin medium */
.p-lg               /* Padding large */
.mt-xl              /* Margin-top extra large */
.mb-sm              /* Margin-bottom small */
```

### Typographie
```css
.text-2xl           /* Taille de texte extra large */
.font-bold          /* Poids de police bold */
.text-center        /* Alignement centré */
.uppercase          /* Texte en majuscules */
```

### Layout
```css
.d-flex             /* Display flex */
.flex-col           /* Direction colonne */
.justify-center     /* Justification centrée */
.items-center       /* Alignement centré */
```

### Grille
```css
.grid               /* Display grid */
.grid-cols-3        /* 3 colonnes */
.gap-md             /* Espacement medium */
```

### Dimensions et Espacements
```css
.w-full             /* Largeur 100% */
.h-full             /* Hauteur 100% */
.h-screen           /* Hauteur 100vh */
.min-h-screen       /* Hauteur minimale 100vh */
.gap-xs             /* Espacement très petit */
.gap-sm             /* Espacement petit */
.gap-md             /* Espacement medium */
.gap-lg             /* Espacement large */
.gap-xl             /* Espacement très large */
```

## ✨ Animations

### Classes d'animation
- `fade-in` : Apparition en fondu
- `slide-up` : Glissement vers le haut
- `slide-down` : Glissement vers le bas
- `scale-in` : Animation d'échelle

### Transitions
- `--transition-fast` : 150ms
- `--transition-normal` : 250ms
- `--transition-slow` : 350ms

## 🎭 États et Interactions

### Hover
```css
.hover:bg-primary:hover    /* Fond primary au hover */
.hover:text-white:hover    /* Texte blanc au hover */
.hover:shadow-lg:hover     /* Ombre large au hover */
```

### Focus
```css
.focus:outline-none:focus  /* Supprime l'outline */
.focus:ring:focus          /* Anneau de focus */
```

## 🔧 Personnalisation

### Modifier les couleurs
Éditez les variables CSS dans `:root` :

```css
:root {
  --color-primary: #VOTRE_COULEUR;
  --color-secondary: #VOTRE_COULEUR;
}
```

### Ajouter de nouvelles couleurs
```css
:root {
  --color-custom: #FF6B6B;
}

.bg-custom { background-color: var(--color-custom); }
.text-custom { color: var(--color-custom); }
```

### Modifier les espacements
```css
:root {
  --spacing-custom: 2.5rem;
}

.p-custom { padding: var(--spacing-custom); }
.m-custom { margin: var(--spacing-custom); }
```

## 📱 Compatibilité

- **Navigateurs** : Chrome, Firefox, Safari, Edge (versions récentes)
- **Mobile** : iOS Safari, Chrome Mobile
- **CSS Grid** : Supporté par tous les navigateurs modernes
- **CSS Variables** : Supporté par tous les navigateurs modernes

## 🚀 Performance

- **Taille** : CSS optimisé et minifiable
- **Classes** : Système de classes utilitaires efficace
- **Animations** : Utilise `transform` et `opacity` pour de meilleures performances
- **Responsive** : Media queries optimisées



## 📖 Exemples d'Usage

### Navigation
```html
<nav class="bg-primary text-white p-md">
    <div class="container d-flex justify-between items-center">
        <h1 class="text-xl font-bold">Logo</h1>
        <div class="d-flex gap-md">
            <a href="#" class="text-white hover:text-gray-light">Accueil</a>
            <a href="#" class="text-white hover:text-gray-light">À propos</a>
            <a href="#" class="text-white hover:text-gray-light">Contact</a>
        </div>
    </div>
</nav>
```

### Formulaire de contact
```html
<form class="max-w-md mx-auto">
    <div class="form-group">
        <label class="form-label">Nom</label>
        <input type="text" class="form-input" required>
    </div>
    
    <div class="form-group">
        <label class="form-label">Email</label>
        <input type="email" class="form-input" required>
    </div>
    
    <div class="form-group">
        <label class="form-label">Message</label>
        <textarea class="form-input" rows="4" required></textarea>
    </div>
    
    <button type="submit" class="btn btn-primary w-full">Envoyer</button>
</form>
```

## 🎯 Bonnes Pratiques

1. **Mobile First** : Commencez toujours par le design mobile
2. **Classes utilitaires** : Utilisez les classes préexistantes plutôt que de créer du CSS personnalisé
3. **Responsive** : Testez sur différents écrans et orientations
4. **Accessibilité** : Utilisez les classes `sr-only` pour le contenu accessible
5. **Performance** : Évitez d'ajouter trop de classes sur un seul élément

## 🔄 Mise à Jour

Pour mettre à jour le kit UI :

1. Sauvegardez vos modifications personnalisées
2. Remplacez `styles.css` par la nouvelle version
3. Réappliquez vos personnalisations
4. Testez sur tous vos projets

## 📞 Support

Ce kit UI est conçu pour être simple et intuitif. Si vous avez des questions :

1. Consultez la page de démonstration (`demo.html`)
2. Vérifiez les exemples dans ce README
3. Inspectez le code CSS pour comprendre la structure

---

**Créé avec ❤️ par LorenzoRU**
# kitUI
