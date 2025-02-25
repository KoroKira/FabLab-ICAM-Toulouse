# Guide d'Utilisation d'Orca Slicer pour Flashforge Adventurer 5M 🖨️

## **Installation et Configuration**
1. **Télécharger Orca Slicer** : Disponible sur [le site officiel](https://github.com/SoftFever/OrcaSlicer).
2. **Sélectionner l'Imprimante** :
   - Dans Orca Slicer, ajoutez une imprimante > Cherchez **Flashforge Adventurer 5M**.
   - Utilisez le profil prédéfini "Flashforge Adventurer 5M" pour des paramètres optimaux.
3. **Calibrage** :
   - Niveaulez le plateau automatiquement via l'option **Bed Leveling**.
   - Ajustez le **Z-offset** si nécessaire (0.1 à 0.2 mm pour une bonne adhérence).

---

## **Paramètres d'Impression Clés**
### **Général**
- **Hauteur de Couche (Layer Height)** :
  - Standard : **0.2 mm**.
  - Haute qualité : **0.1 mm** (temps d'impression + long).
- **Vitesse d'Impression** :
  - Par défaut : **60 mm/s** (augmentez progressivement pour tester la stabilité).
- **Remplissage (Infill)** :
  - **15-30%** : Suffisant pour la plupart des pièces (au-delà, résistance mécanique non améliorée).
  - Motif recommandé : **Gyroïde** (bon compromis résistance/temps).

### **Support**
- **Activer les supports** :
  - Pour surplombs > **45°**.
  - Type : **Arborescent (Tree)** pour économiser du matériel.

### **Refroidissement**
- **Ventilateurs** :
  - **100%** pour le PLA après la première couche.
  - **50-70%** pour le PETG (éviter les déformations).

### **Matériaux**
- **PLA** :
  - Température buse : **200-210°C**.
  - Plateau : **50-60°C**.
- **PETG** :
  - Température buse : **220-235°C**.
  - Plateau : **70-80°C**.

---

## **Conseils d'Impression**
### **Résistance Mécanique**
- **Éviter le sur-remplissage** : Au-delà de **30%**, le gain de résistance est faible, mais le temps et le gaspillage augmentent.
- **Orientation des pièces** :
  - Imprimez les pièces porteuses **perpendiculairement aux forces** appliquées (ex : axes en vertical).

### **Trous de Vis**
- **Diamètre** :
  - Pour des vis M3 : percez **2.8 mm** (ajustement serré) ou **3.0 mm** (ajustement libre).
  - Ajoutez un **chanfrein** (0.5 mm) pour faciliter l'insertion.
- **Astuce Pro** :
  - Utilisez des **inserts thermorétractables** pour une résistance accrue (percez 4.0 mm pour un insert M3).

### **Adhérence au Plateau**
- **Nettoyage** : Utilisez de l'**alcool isopropylique** avant chaque impression.
- **Bordure (Brim)** : Activez-la pour les petites pièces ou celles avec peu de surface de contact.

---

## **Dépannage Rapide**
| **Problème**              | **Solution**                          |
|---------------------------|---------------------------------------|
| Décollage de la pièce     | Augmentez la température du plateau. |
| Filament qui boucle       | Baissez la température de la buse.   |
| Couches décalées          | Serrez les courroies et vérifiez les axes. |

---

# Guide CATIA pour Débutants 🖥️

## **Interface de Base**
- **Arbre de Conception** : Gère l'historique des opérations (renommez les features pour plus de clarté).
- **Workbenches** :
  - **Part Design** : Pièces 3D.
  - **Assembly Design** : Assemblage de pièces.
  - **Drafting** : Plans techniques.

---

## **Conseils de Modélisation**
### **Esquisses (Sketches)**
- **Contraintes** : Toujours **contraindre complètement** l'esquisse (icône "Contraintes" en vert).
- **Outils utiles** :
  - **Symétrie** : Utilisez l'axe de symétrie pour gagner du temps.
  - **Chanfreins/Arrondis** : Ajoutez-les en fin de conception pour éviter les erreurs.

### **Trous Filetés**
- **Ne modélisez pas les filets** :
  - Utilisez l'annotation **Filetage** dans le module Drafting.
  - Percez un **trou lisse** et spécifiez le diamètre nominal (ex : M3 → perçage 2.5 mm).

### **Assemblages**
- **Contraintes** :
  - Utilisez **Coincidence**, **Contact**, et **Offset** pour positionner les pièces.
  - Évitez les contraintes redondantes pour simplifier les calculs.

---

## **Bonnes Pratiques**
- **Gestion de l'Arbre** :
  - Renommez les features (ex : "Plaque_Base" au lieu de "Pad.1").
  - Groupez les opérations logiques (ex : "Détails_Vis").
- **Sauvegardes** :
  - Utilisez **Save Management** pour éviter les fichiers corrompus.
  - Versionnez vos fichiers (ex : "Voiture_V1", "Voiture_V2").

---

## **Astuces de Pro**
- **Paramétrisation** :
  - Utilisez des **formules** pour lier les cotes (ex : Diamètre_Trou = Diamètre_Vis + 0.2 mm).
- **Configurations** :
  - Créez des **configurations** pour tester plusieurs variantes d'une pièce (ex : épaisseurs différentes).