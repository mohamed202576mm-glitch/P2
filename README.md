# Classification binaire avec Keras

Petit projet de classification binaire en Deep Learning pour m'entraîner avec TensorFlow et Keras.

## Fonctionnement
L'objectif est de prédire une catégorie binaire (0 ou 1) à partir d'un ensemble de variables d'entrée.

## Architecture du modèle
J'ai mis en place un réseau de neurones séquentiel (MLP) adapté à la classification :
- Une normalisation des entrées (`BatchNormalization`).
- Des couches cachées avec activation ReLU et du `Dropout` pour limiter le surapprentissage.
- Une couche de sortie avec un seul neurone et une fonction d'activation `sigmoid` pour obtenir une probabilité entre 0 et 1.
- Une compilation basée sur la perte `binary_crossentropy` et un `EarlyStopping` pour automatiser l'arrêt de l'entraînement.

## Bibliothèques utilisées
- Python
- TensorFlow / Keras
- Pandas / Matplotlib
