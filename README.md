# 🧠 Détection de Tumeurs Cérébrales via CNN

Ce projet a été réalisé dans le cadre d’un module d’intelligence artificielle appliquée à la santé. Il vise à développer un modèle capable de détecter automatiquement les types de tumeurs cérébrales à partir d’images IRM.

## 📌 Objectif
Accélérer le diagnostic médical grâce à un modèle prédictif basé sur le deep learning, capable d’identifier les tumeurs suivantes :
- Gliome tumor
- Meningioma tumor
- Pituitary tumor
- No tumor

## 🛠️ Méthodologie

### 1. Analyse des données
- Ensemble de données IRM structuré par dossier.
- Prétraitement des images (redimensionnement, normalisation, encodage).
- Analyse de la distribution des classes.

### 2. Modèle prédictif
- Utilisation d’un **CNN** (Convolutional Neural Network).
- Augmentation des données (rotation, zoom, flip) pour améliorer la robustesse.
- Entraînement sur Google Colab.

### 3. Mise à l’échelle
- Pipeline généralisable à d'autres ensembles IRM.
- Export du modèle en `.h5` ou `SavedModel` pour déploiement.
- Code adaptable à une application web ou mobile.

## ⚙️ Structure du projet

```bash
📁 brain-tumor-detection/
├── brain_tumor_classification.ipynb  # Notebook principal
├── /datasets                         # Images organisées par classes
├── /models                           # Sauvegarde du modèle entraîné
├── README.md                         # Description du projet
```
## Résultats obtenus
Accuracy sur jeu de test : 37.82%
F1-score pondéré : 30.13%
Les performances restent limitées à cause du manque de ressources (GPU limité sur Colab).
Meilleure détection observée pour les tumeurs de type meningioma et pituitary.
**Limite technique :**  L’accès aux GPU sur Google Colab étant restreint, nous n’avons pas pu entraîner le modèle sur plusieurs époques ou architectures plus complexes.


