# 🔬 Skin-Cancer-Classifier-PyTorch : Assistant Diagnostique (Format Notebook)

## 💡 Description du Projet

Ce projet implémente un pipeline complet d'apprentissage profond (*Deep Learning*) pour la **classification binaire d'images** (maligne/bénigne) de lésions cutanées. Il est intégralement contenu dans un seul **Notebook Jupyter/Colab**, permettant une exécution séquentielle et une reproductibilité maximale.

Le projet utilise le **Transfer Learning** avec des architectures de pointe (ResNet-50, EfficientNet-B0) et se conclut par une interface de démonstration interactive via Gradio.

## 🚀 Exécution et Déploiement

Le projet est conçu pour être exécuté étape par étape :

1.  **Exécution Séquentielle :** Le notebook doit être exécuté cellule par cellule, dans l'ordre, pour garantir que les modèles et les fonctions soient correctement définis avant l'entraînement et l'inférence.
2.  **Préparation des Données :** L'exécution réussie dépend de la présence d'un dossier `/data` contenant les sous-dossiers `/train`, `/val` et `/test` (chacun divisé en classes `benign` et `malignant`).
3.  **Démonstration Gradio :** La dernière cellule lance l'application Gradio directement dans l'interface du notebook (ou via un lien public/local), permettant de tester les modèles avec des images téléchargées.

## 🎯 Fonctionnalités Clés

| Étape du Notebook | Rôle Principal | Algorithmes Implémentés |
| :--- | :--- | :--- |
| **Cellule 3 & 4** | **Modélisation & Data** | Architectures **ResNet-50** / **EfficientNet-B0** / CNN Custom. Transformations d'images et augmentation de données. |
| **Cellule 5** | **Entraînement** | **Finetuning** via PyTorch, stratégie de gel des couches, optimisation **Adam**, boucle d'entraînement/validation. |
| **Cellule 6** | **Évaluation** | Calcul de la Matrice de Confusion, **Courbe ROC et AUC**, détermination du **seuil optimal** pour la classification. |
| **Cellule 7** | **Application Démo** | Interface interactive **Gradio** pour l'inférence en temps réel sur image fournie par l'utilisateur. |

