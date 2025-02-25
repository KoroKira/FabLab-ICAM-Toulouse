# Guide de Découpe Laser avec xtool P2 et Préparation de Fichiers SVG 🔥✂️

---

## **Sécurité Avant Tout !**
- **Équipement obligatoire** :
  - Lunettes de protection laser (spécifiques à la longueur d'onde du laser, souvent 455nm ou 1064nm).
  - Ventilation adaptée (activateur d'extraction de fumées).
  - **Ne jamais laisser la machine sans surveillance** (risque d'incendie).
- **Matériaux interdits** :
  - PVC (émet du chlore toxique), Cuir, Fibre de verre, Polystyrène expansé.

---

## **Logiciel et Configuration xtool P2**
1. **Télécharger XCS (xtool Creative Space)** :
   - Disponible sur [le site xtool](https://www.xtool.com/software).
   - Sélectionnez le modèle **P2** dans les paramètres.
2. **Connexion** :
   - Wi-Fi ou USB (préférez USB pour une connexion stable).
3. **Mise à jour du firmware** :
   - Vérifiez les mises à jour dans XCS > "Machine Settings".

---

## **Préparation du Fichier SVG**
### **Règles de Base**
- **Vectorisez tout** :
  - Convertir les textes et formes en tracés vectoriels (Outline Stroke dans Illustrator/Inkscape).
  - **Évitez les bitmaps** (sauf pour la gravure raster).
- **Formats** :
  - Exportez en **SVG** (préférable) ou DXF.
  - Résolution : **300 DPI** minimum pour la gravure détaillée.

### **Paramètres des Traits**
- **Découpe Laser** :
  - Traits **0.001 mm d'épaisseur** (ou "Hairline" dans les logiciels).
  - Couleur : **Rouge (#FF0000)** pour les coupes, **Bleu (#0000FF)** pour les gravures profondes.
- **Gravure** :
  - Utilisez des zones **remplies en noir** (ou nuances de gris pour varier l'intensité).

### **Bonnes Pratiques**
1. **Vérifiez les chemins fermés** :
   - Les formes doivent être fermées (pas de "trous" dans les tracés).
2. **Évitez les superpositions** :
   - Les lignes qui se chevauchent peuvent causer des brûlures.
3. **Dimensions du matériau** :
   - Définissez la taille de la plaque dans XCS (ex : 600x400mm pour le P2).
4. **Origine (0,0)** :
   - Positionnez votre design dans le coin inférieur gauche du canevas.

---

## **Configuration de la Machine**
1. **Placement du matériau** :
   - Fixez-le avec des pinces ou du ruban adhésif double-face (évitez les bulles d'air).
2. **Mise au point (Focus)** :
   - Utilisez la **fonction auto-focus** du P2 (la tête laser mesure automatiquement l'épaisseur).
3. **Test de découpe** :
   - Lancez un test sur un coin du matériau avec un carré de 10x10mm.

---

## **Paramètres de Découpe/Gravure (Exemples)**
| **Matériau**      | **Épaisseur** | **Puissance** | **Vitesse** | **Passes** |
|--------------------|---------------|---------------|-------------|------------|
| **Bois (plywood)** | 3mm           | 80%           | 30mm/s      | 1          |
| **Acrylique**      | 5mm           | 70%           | 15mm/s      | 2          |
| **Carton**         | 2mm           | 40%           | 100mm/s     | 1          |
| **Gravure sur métal** | -        | 100%          | 5mm/s       | 3          |

- **Astuce** :
  - Consultez la **base de données matériaux** intégrée à XCS pour des réglages optimaux.
  - Commencez toujours par des tests sur des chutes !

---

## **Problèmes Courants et Solutions**
| **Problème**               | **Cause Probable**        | **Solution**                      |
|----------------------------|---------------------------|-----------------------------------|
| Découpe incomplète         | Puissance trop faible     | Augmentez la puissance ou passes. |
| Bords brûlés               | Vitesse trop lente        | Augmentez la vitesse.             |
| Gravure inégale            | Matériau non plat         | Aplatissez avec un poids.         |
| Erreur de focalisation     | Capteur sale              | Nettoyez la lentille/capteur.     |

---

## **Astuces Pro**
1. **Utilisez des "jigs"** :
   - Créez un gabarit en MDF pour positionner des pièces récurrentes.
2. **Gravure avant découpe** :
   - Gravez d'abord, puis découpez pour éviter les déplacements.
3. **Masquage** :
   - Appliquez du ruban de masquage sur l'acrylique pour éviter les rayures.
4. **Nettoyage** :
   - Passez un chiffon microfibre sur la lentille après chaque utilisation.

---

## **Exemple de Workflow**
1. Dessinez dans Illustrator/Inkscape → Export SVG.
2. Importez dans XCS → Assignez couleurs/paramètres.
3. Calibrez la machine → Testez sur un coin.
4. Lancez la découpe → Surveillez les premières secondes.
5. Post-traitement : Ponçage léger, assemblage.
