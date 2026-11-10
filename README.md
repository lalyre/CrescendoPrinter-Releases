# CrescendoPrinter — téléchargements

Copyright © 2026 Claude Lalyre

Application Windows 64 bits pour préparer des PDF d’impression de jeux sur les bulletins officiels Crescendo.

## Télécharger la version 0.0.1

- [Télécharger le ZIP complet (EXE, exemple, instructions et licence)](https://github.com/lalyre/CrescendoPrinter-Releases/releases/download/v0.0.1/CrescendoPrinter-0.0.1.zip)
- [Télécharger CrescendoPrinter.exe](https://github.com/lalyre/CrescendoPrinter-Releases/releases/download/v0.0.1/CrescendoPrinter.exe)
- [Notes de version et fichiers joints](https://github.com/lalyre/CrescendoPrinter-Releases/releases/tag/v0.0.1)
- [Fichier d’exemple : six jeux pour deux pages](exemples/jeux-crescendo.txt)

Pour le ZIP, extraire tous les fichiers puis suivre `LISEZMOI.txt`.

Aucune installation de Python n’est nécessaire. Télécharger l’EXE, puis le lancer.

## Utilisation

1. Cliquer sur **Charger un fichier de jeux…** et sélectionner un fichier texte.
2. Cliquer sur **Générer le document PDF…** et choisir où l’enregistrer.
3. Ouvrir le document dans un lecteur PDF et appliquer les réglages ci-dessous avant d’imprimer.

Le fichier contient un jeu par ligne : **10 numéros distincts entre 1 et 25**, séparés par des espaces, des points-virgules ou des tirets. Les lignes vides sont ignorées. En cas de ligne invalide, une fenêtre indique son numéro.

```text
1;3;5;7;9;11;13;15;20;25
2 4 6 8 10 12 14 16 18 24
1-2-3-4-5-6-7-8-9-10
```

Les jeux sont imprimés dans l’ordre du fichier, jusqu’à cinq par page. Les grilles inutilisées sur la dernière page restent vides. **150 jeux produisent 30 pages.**

## Paramètres d’impression

- **Taille réelle / échelle : 100 %.**
- **Sans ajustement à la page.**
- **Format papier personnalisé : largeur 160 mm × hauteur 152 mm.**
- Sans agrandissement sans bordure et sans recto verso.
- Une page PDF par bulletin ; respecter le sens d’insertion.

Le PDF conserve le format initial de calibrage **160 × 149 mm**. Le format papier **160 × 152 mm** est le réglage rapporté comme satisfaisant par Math06 lors du test de calibrage.

Les tirages et le nombre de samedis sont à cocher manuellement sur les bulletins. Cette première version est destinée aux essais : l’alignement et la répétabilité de l’impression en série restent à confirmer sur les bulletins réels.

## Licence

[Apache License 2.0](LICENSE).

Projet indépendant, sans partenariat établi avec FDJ ou le groupement À nous les millions.
