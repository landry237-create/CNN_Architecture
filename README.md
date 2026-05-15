# CNN_Architecture

# Classification d'Images avec CNN (PyTorch)




Ce projet implémente un Réseau de Neurones Convolutif (CNN) performant en utilisant **PyTorch** pour la classification automatisée d'images de mode. 

**Auteur :**  Landry NOUMBISSI  
**Statut :** Master 2 Recherche en Science des Données & IA

---

## 📊 Présentation du Projet
L'objectif est de classifier les articles vestimentaires du dataset **Fashion-MNIST**. Le modèle traite des images en niveaux de gris de $28 \times 28$ pixels pour les assigner à l'une des 10 catégories prédéfinies.

### Points Clés :
- **Précision atteinte :** ~85,99% sur le jeu d'entraînement.
- **Framework :** PyTorch.
- **Backend :** Support GPU (CUDA) intégré.

---

## 📂 Jeu de Données
Le modèle utilise le dataset **Fashion-MNIST** (via `fashion-mnist_train.csv`).
- **Volume :** 60 000 échantillons d'entraînement.
- **Dimensions :** $28 \times 28$ pixels (784 caractéristiques).
- **Classes :** 10 (T-shirt, Pantalon, Pull, Robe, Manteau, Sandale, Chemise, Basket, Sac, Bottine).

!

---

## 🏗️ Architecture du Modèle
Le réseau est conçu avec une structure CNN classique optimisée :

1. **Couches Convolutives :** Pour l'extraction de motifs spatiaux (bordures, textures).
2. **Activation ReLU :** Pour introduire la non-linéarité.
3. **Max Pooling :** Pour réduire la résolution spatiale et extraire les caractéristiques dominantes.
4. **Couches Denses (Fully Connected) :** Pour la classification finale.

---

## 🚀 Installation et Utilisation

### Prérequis
Clonez le dépôt et installez les bibliothèques nécessaires :

```bash
pip install torch torchvision pandas numpy matplotlib
