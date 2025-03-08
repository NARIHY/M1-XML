# Travaux dirigés : Analyse et manipulation de données XML

Nous travaillons pour une librairie en ligne qui stocke ses infos de livres dans un fichier XML.  
Notre tâche consiste à analyser ce fichier et à extraire les informations spécifiques pour générer un rapport.

## 1. Commençons par les étapes pour créer manuellement la structure du fichier XML

### a. Déclaration XML

- Écrire la ligne qui spécifie la version XML et l'encodage du fichier.

### b. Élément racine

- Créer un élément racine. C'est l'élément qui englobera tous les autres éléments du fichier XML.

### c. Créer le premier élément `book` avec l'attribut `category` défini sur "fiction"

- L'élément `book` doit contenir un attribut `category` avec la valeur "fiction".

### d. Créer l'élément `title` avec l'attribut `lang` défini sur "fr" et le texte "Le guide du voyageur galactique"

- L'élément `title` doit avoir un attribut `lang` avec la valeur "fr" et le texte "Le guide du voyageur galactique".

### e. Créer l'élément `author` avec le texte "Douglas Adams"

- L'élément `author` doit contenir le texte "Douglas Adams".

### f. Créer l'élément `year` avec le texte 1979

- L'élément `year` doit contenir l'année de publication, soit 1979.

### g. Créer l'élément `price` avec le texte 8,99 $

- L'élément `price` doit contenir le texte "8,99 $".

### i. Fermer l'élément `book`

- Fermer l'élément `book` pour compléter la structure de l'entrée de ce livre.

## 2.  Analyse et Extraction de Données XML

## Description

Ce projet consiste à analyser et extraire des informations d'un fichier XML contenant des données sur des livres. À l'aide de Python et de la bibliothèque `xml.etree.ElementTree`, nous allons charger et analyser le fichier XML `books.xml`, puis extraire des informations telles que les titres et auteurs des livres, ainsi que d'autres données pertinentes, et enfin générer un rapport avec ces informations.

## Objectifs

1. **Chargement et analyse du fichier XML** : Utilisation de la bibliothèque `xml.etree.ElementTree` pour charger et analyser le fichier `books.xml`.
2. **Extraction d'informations** :
   - Afficher les titres et les auteurs de tous les livres.
   - Extraire et afficher les titres des livres de la catégorie "technology".
   - Calculer et afficher le prix moyen des livres.
   - Trouver et afficher le titre du livre le plus ancien.
3. **Génération d'un rapport** :
   - Créer un rapport listant tous les livres avec leur titre, auteur, année de publication et prix.
   - Ajouter une section dans le rapport pour afficher le prix moyen des livres et le titre du livre le plus ancien.

## Structure du Projet

```
Analyse-Extraction-XML/
├── books.xml
├── extraction/extract-devoir.py
└── sujet.md
```

- **`books.xml`** : Fichier XML contenant les informations sur les livres.
- **`extract-devoir.py`** : Script Python utilisé pour analyser et extraire les données du fichier XML.
- **`sujet.md`** : Ce fichier, contenant la description et les instructions du projet.

## Étapes à Suivre

1. **Chargement et Analyse du Fichier XML** :
   - Le fichier XML doit être chargé à l’aide de la bibliothèque `xml.etree.ElementTree` en Python.
   - Vous devez analyser la structure du fichier XML pour en extraire les informations nécessaires.

2. **Extraction des Données** :
   - Extraire les titres et auteurs de tous les livres dans le fichier XML.
   - Filtrer les livres par catégorie (par exemple, la catégorie "technology").
   - Calculer le prix moyen des livres.
   - Identifier le livre le plus ancien en fonction de l'année de publication.

3. **Génération du Rapport** :
   - Générer un rapport qui liste tous les livres, avec leur titre, auteur, année de publication et prix.
   - Ajouter une section qui indique le prix moyen des livres et le titre du livre le plus ancien.

## Exemple de Code

Voici un exemple de script Python pour charger et analyser le fichier XML :

```python
import xml.etree.ElementTree as ET

# Chargement et analyse du fichier XML
tree = ET.parse('books.xml')
root = tree.getroot()

# Exemple : Afficher les titres et auteurs
for book in root.findall('book'):
    title = book.find('title').text
    author = book.find('author').text
    print(f"Titre : {title}, Auteur : {author}")
```

## Prérequis

- Python 3.x
- La bibliothèque `xml.etree.ElementTree` (incluse dans la bibliothèque standard de Python).

## Instructions d'Utilisation

1. Clonez ce dépôt ou téléchargez les fichiers.
2. Placez le fichier `books.xml` dans le même répertoire que le script `extract_data.py`.
3. Exécutez le script Python pour commencer l'analyse et l'extraction des données.

```bash
python extract_data.py
```