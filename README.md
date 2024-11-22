# **Segmentation d'Images Supervisée avec SVM**

## **Description**
Ce projet propose une méthode de segmentation d'image supervisée en utilisant un modèle basé sur les **SVM (Support Vector Machines)**. Deux approches distinctes ont été explorées pour extraire les caractéristiques des pixels et entraîner les modèles, en exploitant des informations colorimétriques (RGB et HSV) ainsi que des intensités en niveaux de gris.

La segmentation est effectuée sur la base d'un masque binaire, permettant de distinguer les régions d'intérêt dans les images.

---

## **Objectifs**
- Implémenter une segmentation d'image supervisée à l'aide de SVM.
- Comparer les performances de deux approches distinctes :  
  1. Caractéristiques dans les espaces colorimétriques RGB et HSV.  
  2. Caractéristiques basées uniquement sur les niveaux de gris.
- Évaluer les performances avec des métriques numériques et une visualisation qualitative.

---

## **Points Principaux**

### **1. Approches Implémentées**
#### **a) Première approche : RGB + HSV**
- **Extraction des caractéristiques** : Les pixels sont décrits par leurs valeurs dans les espaces **RGB** et **HSV**.
- **Modélisation supervisée** : Un modèle SVM est entraîné sur les caractéristiques des pixels, avec des étiquettes générées à partir d'un masque binaire.
- **Évaluation** : Le modèle est testé sur une image différente et ses performances sont évaluées avec des métriques telles que :
  - **Précision (Accuracy)**  
  - **Rappel (Recall)**  
  - **Score F1 (F1-Score)**  
- **Résultats visuels** : Affichage de masques segmentés.

#### **b) Deuxième approche : Niveaux de gris**
- **Extraction des caractéristiques** : Les intensités en niveaux de gris des pixels sont utilisées comme caractéristiques d'entrée.
- **Modélisation supervisée** : Un modèle SVM est entraîné et évalué avec la même méthodologie que pour la première approche.

---

## **Résultats**

| Approche        | Précision | Rappel | F1-Score |
|------------------|-----------|--------|----------|
| RGB + HSV        | 95%       | 92%    | 93.5%    |
| Niveaux de gris  | 90%       | 85%    | 87.5%    |

Les masques segmentés montrent que l'approche **RGB+HSV** donne de meilleurs résultats, notamment pour des images complexes avec des variations de couleur.

---

## **Auteur**
- [lamdibih khadija]  
