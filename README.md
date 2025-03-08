# M1-XML

## Description

Le projet **M1-XML** est conçu pour organiser les cours du programme de Master 1 en XML. Chaque cours sera placé dans un dossier spécifique à la date et à l'année du cours. Les dossiers seront nommés sous le format suivant : **date-moi-année** (par exemple, **08-03-2025** pour un cours ayant lieu le 8 mars 2025).

## Structure du Projet

La structure des dossiers et fichiers du projet est organisée de la manière suivante :

```
M1-XML/
├── 08-03-2025/
│   ├── Cours_1.xml
│   └── Cours_2.xml
├── 15-03-2025/
│   └── Cours_3.xml
└── 22-03-2025/
    ├── Cours_4.xml
    └── Cours_5.xml
```

- **Chaque dossier** : Représente un cours ou une session spécifique, et est nommé sous le format `jj-mm-aaaa` pour refléter la date du cours.
- **Chaque fichier XML** : Contient les informations pertinentes du cours (contenu du cours, liens, exercices, etc.).

## Comment ajouter un cours

1. Créez un dossier en suivant la structure de date `jj-mm-aaaa` correspondant à la date du cours.
2. Dans ce dossier, ajoutez les fichiers XML qui contiendront les informations relatives aux différents cours dispensés ce jour-là.
3. Chaque fichier XML doit être nommé de manière à refléter le contenu du cours (par exemple, `Cours_1.xml`, `Exercice_1.xml`, etc.).

## Technologies utilisées

- **XML** : Format de données utilisé pour structurer et organiser les informations du cours.
- **Système de fichiers** : Organisation des cours par date et année dans des dossiers dédiés.

## Contribution

Si vous souhaitez contribuer à ce projet :

1. Forkez ce dépôt.
2. Créez une nouvelle branche pour votre fonctionnalité (`git checkout -b feature-nom-de-la-fonctionnalité`).
3. Commitez vos modifications (`git commit -am 'Ajout d'un nouveau cours'`).
4. Poussez la branche (`git push origin feature-nom-de-la-fonctionnalité`).
5. Ouvrez une pull request.

## License

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.
