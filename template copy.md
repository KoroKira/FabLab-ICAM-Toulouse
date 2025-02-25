---
# En-tête YAML (optionnel mais utile pour la métadata)
title: "Guide Laser xtool P2"
author: "[Nom]"
date: "2024-02-20"
version: "1.0"
---

<!-- ==================== -->
<!-- ZONE DE DOCUMENTATION -->
<!-- ==================== -->

# Guide de Découpe Laser - xtool P2 🔥

<!-- Commentaire : 
  - Garder le ton professionnel mais accessible
  - Utiliser emojis modérément pour aérer le texte
-->

## 🔧 Configuration Machine

<!-- Commentaire :
  - Décrire les paramètres PHYSIQUES de la machine
  - Inclure des captures si nécessaire
-->

```yaml
# Paramètres de base (à compléter)
Focal Length: <!-- ✂️ (ex: 2.5") -->
Work Area: 600x400mm
Laser Type: Diode 20W
```

![Schéma machine](lien_image.png) <!-- Remplacer par chemin réel -->

## ⚠️ Sécurité

<!-- Commentaire : 
  - Lister les dangers principaux
  - Être très visuel sur les interdits
-->

<div class="danger">

### ❌ ABSOLUMENT INTERDIT
- PVC (émet du **chlore toxique**)
- Cuir animal
- Matériaux réfléchissants

</div>

### Équipement Obligatoire
- [ ] Lunettes laser OD6+ <!-- Case à cocher -->
- [ ] Ventilation externe
- [ ] Gants anti-coupure

## 📁 Préparation Fichiers

<!-- Commentaire :
  - Donner des exemples concrets
  - Inclure des snippets de code
-->

### Règles SVG
```svg
<!-- Exemple de structure SVG propre -->
<svg>
  <path 
    fill="none" 
    stroke="#FF0000" <!-- Découpe -->
    stroke-width="0.001mm"
    d="..."
  />
</svg>
```

| Élément  | Couleur    | Épaisseur | Description           |
|----------|------------|-----------|-----------------------|
| Découpe  | `#FF0000`  | 0.001mm   | Contour principal     |
| Gravure  | `#0000FF`  | -         | Zones remplies        |

## 🛠 Paramètres Matériaux

<!-- Commentaire :
  - Compléter le tableau avec valeurs testées
  - Garder unités cohérentes
-->

| Matériau       | Épaisseur | Puissance | Vitesse | Passes | Note                                  |
|----------------|-----------|-----------|---------|--------|---------------------------------------|
| Contreplaqué   | 3mm       | 85%       | 30mm/s  | 1      | <!-- ✂️ (ex: Utiliser masquage) -->   |
| Acrylique      | 5mm       | 75%       | 20mm/s  | 2      |                                       |

## 💡 Bonnes Pratiques

<!-- Commentaire :
  - Ajouter des astuces testées en atelier
  - Inclure des pièges courants
-->

```markdown
1. [Test obligatoire] Toujours faire un "Fire Test" sur un coin
2. [Optimisation] Graver avant découpe pour éviter le mouvement
3. [Réglage] 0.1mm de jeu pour les assemblages serrés
```

## 🚨 Dépannage

<!-- Commentaire :
  - Lister problèmes fréquents
  - Solutions concrètes et vérifiées
-->

### Découpe Incomplète
```diagnostic
Cause probable : Lentille sale → Nettoyer avec alcool isopropylique
```

### Bords Brûlés
```corrective-action
1. Baisser puissance de 10%
2. Augmenter vitesse
3. Ajouter couche de masquage
```

## 📚 Ressources

<!-- Commentaire :
  - Lier documents externes
  - Références techniques
-->

- [Fiche sécurité xtool](lien.pdf)
- [Profile Material XCS](lien.conf)
- [Norme EN 60825-1](lien)

<!-- ============== -->
<!-- ZONE DE DONNEES -->
<!-- ============== -->

%% Vous pouvez écrire ici des notes privées pour les rédacteurs %%
<!-- 
  TODO:
  - Compléter section Acrylique
  - Vérifier valeurs laser 20W
  - Ajouter photos montage
-->