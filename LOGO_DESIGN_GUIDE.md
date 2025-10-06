# Guide de Design des Logos - ART DE LA TAILLE

## 🎨 Disposition actuelle

Les logos sont maintenant disposés **à gauche de la page**, **à la même hauteur**, chacun dans un **cercle élégant**.

## 📐 Structure HTML

```html
<div class="logo-container">
  <div class="logo-wrapper">
    <img src="assets/logos/logo-artdelataille.png" alt="ART DE LA TAILLE" class="main-logo">
  </div>
  <div class="logo-wrapper">
    <img src="assets/logos/logo-jardicoop.png" alt="JARDICOOP" class="partner-logo">
  </div>
</div>
```

## 🎯 Styles CSS principaux

### Container des logos
- **Alignement** : `justify-content: flex-start` (à gauche)
- **Espacement** : `gap: 25px` entre les logos
- **Responsive** : `flex-wrap: wrap` pour mobile

### Cercles élégants
- **Taille** : `100px × 100px` (desktop)
- **Forme** : `border-radius: 50%` (cercle parfait)
- **Bordure** : `3px solid var(--accent-green)`
- **Fond** : Dégradé `var(--light-beige)` vers `var(--warm-beige)`
- **Ombre** : `box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15)`

### Logos dans les cercles
- **Logo principal** : `70px × 70px` maximum
- **Logo partenaire** : `60px × 60px` maximum
- **Proportions** : `object-fit: contain` (maintient les proportions)

## 📱 Responsive Design

### Tablette (≤ 768px)
- Cercles : `80px × 80px`
- Logo principal : `55px × 55px`
- Logo partenaire : `45px × 45px`
- Alignement : Centré pour un meilleur rendu

### Mobile (≤ 480px)
- Cercles : `70px × 70px`
- Logo principal : `45px × 45px`
- Logo partenaire : `35px × 35px`
- Espacement réduit : `15px`

## 🔧 Ajustements faciles

### Changer l'alignement
```css
.logo-container {
  justify-content: center; /* Pour centrer */
  justify-content: flex-end; /* Pour aligner à droite */
}
```

### Modifier la taille des cercles
```css
.logo-wrapper {
  width: 120px; /* Nouvelle taille */
  height: 120px; /* Doit être identique */
}
```

### Ajuster l'espacement
```css
.logo-container {
  gap: 40px; /* Plus d'espace entre les logos */
}
```

### Changer les couleurs
```css
.logo-wrapper {
  border-color: var(--primary-green); /* Nouvelle couleur de bordure */
  background: linear-gradient(135deg, #couleur1, #couleur2); /* Nouveau dégradé */
}
```

## ✨ Effets visuels

- **Hover** : Translation vers le haut + agrandissement
- **Animation** : Transition fluide de 0.3s
- **Ombre dynamique** : Augmentation de l'ombre au hover
- **Couleur de bordure** : Change au hover

## 🎨 Cohérence visuelle

- Utilise les variables CSS existantes du site
- Respecte la palette de couleurs (verts, beiges)
- Maintient l'harmonie avec le design global
- Effets subtils et professionnels