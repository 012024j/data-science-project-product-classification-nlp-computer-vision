# Classification automatique d’articles e-commerce (Texte & Image)
## Structure du projet
Ce projet s'inscrit dans le cadre de la formation Data Scientist. Il est organisé autour de deux volets complémentaires :

## 1. Classification à partir du texte :
- Prétraitements classiques : nettoyage, lemmatisation, stopwords
- Méthodes NLP basiques : BoW, TF-IDF + réduction de dimension (PCA, t-SNE, UMAP…)
- Méthodes NLP avancées : Word2Vec, BERT, USE + clustering K-Means
- Mesure de performance : ARI (Adjusted Rand Index)

## 2. Classification à partir de l’image :
- Prétraitement des images : conversion N&B, réduction de bruit, normalisation
- Méthodes basiques : SIFT, ORB
- Méthode avancée : CNN (Transfer Learning, VGG16)
- Réduction de dimension et clustering
- Évaluation avec matrice de confusion et ARI

## Étapes clés réalisées
Étape	Description
- 1-Prétraitement des textes & images
- 2-Extraction des features textuelles (BoW, TF-IDF, Word2Vec, BERT, USE)
- 3-Extraction des features visuelles (SIFT, ORB, CNN)
- 4-Réduction de dimension 2D & clustering
- 5-Évaluation des clusters via ARI, analyse de faisabilité
- 6-Classification supervisée avec CNN (avec/sans data augmentation)
- 7-Requête API OpenFoodFacts pour identifier de nouveaux produits

## Résultats principaux
- Texte : les embeddings avancés (USE, Word2Vec) combinés à UMAP ou t-SNE permettent des clusters cohérents (score ARI > 0.45).
- Image : la classification via CNN + UMAP atteint un score ARI de 0.45, confirmant la faisabilité.
- Supervisé (CNN) : précision test avec data augmentation > 80%, démontrant une bonne généralisation.
- API : extraction automatisée de produits d’épicerie fine contenant “Champagne”.

## Outils & Librairies
- Python, Pandas, NumPy, Matplotlib, Seaborn
- Sklearn (PCA, KMeans, ARI)
- NLTK, SpaCy, Gensim
- TensorFlow / Keras (CNN, Transfer Learning)
- OpenCV (prétraitement image, SIFT/ORB)
- UMAP, t-SNE
- API OpenFoodFacts (requests)

## Compétences développées
- Prétraitement de données non structurées (texte & image)
- Feature engineering avancé (Word Embeddings, CNN)
- Réduction de dimension, clustering, évaluation
- Modélisation supervisée en Computer Vision
- Utilisation d’API et automatisation de collecte

## Auteure
- Oumou Faye
- Formation : Data Scientist
- Mentor : Medina Hadjem

