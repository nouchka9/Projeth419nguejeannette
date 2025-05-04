# 🧠 Classification de Radiographies Thoraciques avec un Réseau de Neurones Convolutifs (CNN)

> Projet académique réalisé dans le cadre du cours **PROJ-H-419 – Projet en ingénierie biomédicale (ULB)**.

Ce projet vise à développer un modèle de deep learning pour la **classification automatique de radiographies thoraciques** (X-rays), notamment pour détecter des cas de **pneumonie** à partir d'images médicales.

---

## 📂 Données utilisées

Les données proviennent de la base publique suivante :

- 📎 **Chest X-Ray Images (Pneumonia)** – disponible sur Kaggle  
- 🔗 Lien vers la base de données : [https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

Les données sont divisées en trois sous-dossiers :
- `train/`
- `test/`
- `val/`

Chacun contient deux catégories : `NORMAL` et `PNEUMONIA`.

---

## 💻 Notebook sur Kaggle

Vous pouvez consulter et exécuter ce projet sur Kaggle ici :  
👉 [Lien vers le notebook Kaggle](https://www.kaggle.com/ton-nom-utilisateur/nom-du-notebook) *(remplace par ton lien réel)*

---

## 🛠️ Technologies utilisées

- **Python 3**
- **TensorFlow / Keras**
- NumPy, Matplotlib, Seaborn, scikit-learn
- OpenCV pour le traitement d’image
- Kaggle notebooks pour l’environnement d’exécution

---

## ⚙️ Étapes du projet

1. **Importation des données et visualisation**
2. **Prétraitement des images** :
   - Redimensionnement
   - Normalisation
   - Data Augmentation
3. **Construction du CNN**
   - Couches convolutionnelles, pooling, dropout, fully connected, softmax
4. **Compilation & Entraînement du modèle**
5. **Évaluation des performances**
   - Courbes de précision (accuracy), perte (loss)
   - Matrice de confusion
6. **Prédictions avec taux de confiance**
7. **Analyse des résultats**

---

## 📊 Résultats obtenus

- **Accuracy sur les données de test** : environ 95%
- **F1-score, recall, precision** : affichés dans le notebook
- **Exemples de prédictions** avec images et taux de confiance

---

## 🧠 Structure du CNN (exemple)

```text
Conv2D → ReLU → MaxPooling → Dropout
Conv2D → ReLU → MaxPooling → Dropout
Flatten → Dense → Dropout → Dense (Softmax)
