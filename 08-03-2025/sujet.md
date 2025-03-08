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

