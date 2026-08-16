# TP4 — Recherche d’emploi féminin dans *Le Soir* en 1938 et 1939

Ce dossier contient le notebook réalisé pour le travail final du cours de Traitement automatique de corpus.

## Corpus

Le corpus a été constitué sur la plateforme CAMille avec la requête exacte :

```text
"jeune fille" AND "cherche place"
```

Filtres appliqués :

* journal : *Le Soir* ;
* années : 1938 et 1939.

L’export comprend 903 pages : 496 pour 1938 et 407 pour 1939.

## Contenu

Le fichier `tp4_emploi_feminin.ipynb` comprend :

* l’exploration des métadonnées ;
* l’étude des effets de la requête et des erreurs OCR ;
* l’extraction de passages liés à la recherche d’emploi féminin ;
* l’analyse des fréquences lexicales ;
* l’étude des âges mentionnés ;
* l’extraction de mots-clés avec YAKE ;
* le classement de cinq domaines d’emploi ;
* le contrôle manuel d’échantillons ;
* une comparaison entre 1938 et 1939 ;
* une discussion des limites de l’analyse automatique.

## Données

Le notebook utilise les métadonnées XLSX et les fichiers texte exportés depuis CAMille. Les données doivent être placées dans :

```text
data/tp4_jeune_fille/
```

avec les fichiers texte dans :

```text
data/tp4_jeune_fille/textes/
```

Les données du corpus ne sont pas publiées dans ce dossier.

## Exécution

Le notebook utilise l’environnement Python du dépôt et les dépendances indiquées dans le fichier `requirements.txt`.

