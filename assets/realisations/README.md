# Dossier Réalisations

Ce dossier contient les photos des réalisations d'ART DE LA TAILLE.

## Instructions pour ajouter des photos

1. **Format recommandé** : JPG ou PNG
2. **Dimensions optimales** : 400x300px (ratio 4:3)
3. **Nommage** : Utilisez des noms descriptifs (ex: `elagage-1.jpg`, `cloture-terrasse.jpg`)
4. **Qualité** : Optimisez les images pour le web (compression légère)

## Intégration dans le site

Pour ajouter une photo dans la galerie :

1. Placez l'image dans ce dossier
2. Ouvrez `index.html`
3. Trouvez la section `<!-- Galerie responsive pour les photos -->`
4. Remplacez un `.gallery-placeholder` par :

```html
<div class="gallery-item">
  <img src="assets/realisations/votre-photo.jpg" alt="Description de la réalisation" class="gallery-image">
</div>
```

5. Ajoutez le CSS pour `.gallery-image` si nécessaire :

```css
.gallery-image {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: var(--border-radius);
}
```

## Photos suggérées

- Élagage d'arbres
- Installation de clôtures
- Travaux de pavage
- Création de terrasses
- Jardins complets
- Entretien régulier