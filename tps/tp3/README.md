# TP3 — Clustering et Word2Vec sur le corpus CAMille

Ce TP étudie 1 000 documents du corpus CAMille publiés entre 1930 et 1939.

## Contenu

- `tp3.ipynb` : notebook contenant le clustering et l’analyse Word2Vec ;
- `clusters_1930_1939.png` : représentation des cinq clusters après réduction par PCA.

## Clustering

Les documents sont représentés avec TF-IDF, puis répartis en cinq groupes avec K-means. YAKE est utilisé pour extraire les mots-clés associés à chaque cluster.

Les cinq groupes contiennent respectivement 105, 140, 467, 140 et 148 documents. Les résultats font apparaître des ensembles liés aux programmes radiophoniques, aux annonces immobilières, aux recherches d’emploi et à la vente de biens. Le cluster 2 est plus hétérogène.

## Word2Vec

Trois configurations sont comparées :

- `window=5, min_count=5` ;
- `window=2, min_count=5` ;
- `window=5, min_count=20`.

La troisième configuration est retenue, car le seuil `min_count=20` réduit le poids des formes rares et de certaines erreurs d’OCR. Les voisins de « Paris » et de « ministre » sont interprétables, tandis que ceux de « guerre » sont plus dispersés.

## Données et exécution

Le dossier `data` n’est pas publié sur GitHub en raison de la taille du corpus. L’exécution complète nécessite :

- les fichiers OCR dans `data/txt` ;
- le corpus segmenté en phrases dans `data/sents1.txt` ;
- l’environnement Python `tac_venv`.

Le notebook a été vérifié avec `Restart` puis `Run All`.