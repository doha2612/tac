# TP2 — Exploration du corpus CAMille de 1939

**Étudiante : Doha Belaaroussi**

Ce dossier contient l’analyse de 100 fichiers du corpus CAMille publiés en 1939.

## Fichiers

- `tp2_1939.ipynb` : notebook principal ;
- `nuage_mots_1939.png` : nuage de mots final utilisé dans l’analyse.

## Méthodes

Le notebook applique quatre traitements présentés dans le module 3 :

1. extraction de mots-clés avec YAKE ;
2. nettoyage lexical et création d’un nuage de mots ;
3. reconnaissance des personnes, organisations et lieux avec SpaCy ;
4. analyse de la polarité et de la subjectivité de dix phrases avec TextBlob-FR.

## Corpus

Les 100 fichiers de 1939 sont lus depuis le dossier `data/txt`.

Ils représentent 4 073 198 caractères. Le dossier `data` n’est pas inclus dans le dépôt en raison de la taille du corpus.

## Principaux résultats

YAKE a retenu 951 occurrences de bigrammes. Les résultats montrent la coexistence d’articles politiques, de petites annonces, de programmes radiophoniques et d’informations culturelles. La reconnaissance d’entités fait ressortir plusieurs responsables politiques, agences de presse et lieux belges ou européens. L’analyse de sentiment montre plusieurs écarts entre les scores de TextBlob-FR et le sens global des phrases.

## Exécution

Le notebook utilise l’environnement Python `tac_venv`. Il peut être vérifié avec `Restart` puis `Run All`, à condition que les fichiers du corpus soient présents dans `data/txt`.

