# CrescendoPrinter ? t?l?chargements

Copyright ? 2026 Claude Lalyre

Application Windows 64 bits pour pr?parer des PDF d?impression de jeux sur les bulletins officiels Crescendo.

## T?l?charger la version 0.0.1

- [T?l?charger CrescendoPrinter.exe](https://github.com/lalyre/CrescendoPrinter-Releases/releases/download/v0.0.1/CrescendoPrinter.exe)
- [Notes de version et fichiers joints](https://github.com/lalyre/CrescendoPrinter-Releases/releases/tag/v0.0.1)
- [Fichier d?exemple : six jeux pour deux pages](exemples/jeux-crescendo.txt)

Aucune installation de Python n?est n?cessaire. T?l?charger l?EXE, puis le lancer.

## Utilisation

1. Cliquer sur **Charger un fichier de jeux?** et s?lectionner un fichier texte.
2. Cliquer sur **G?n?rer le document PDF?** et choisir o? l?enregistrer.
3. Ouvrir le document dans un lecteur PDF et appliquer les r?glages ci-dessous avant d?imprimer.

Le fichier contient un jeu par ligne : **10 num?ros distincts entre 1 et 25**, s?par?s par des espaces, des points-virgules ou des tirets. Les lignes vides sont ignor?es. En cas de ligne invalide, une fen?tre indique son num?ro.

```text
1;3;5;7;9;11;13;15;20;25
2 4 6 8 10 12 14 16 18 24
1-2-3-4-5-6-7-8-9-10
```

Les jeux sont imprim?s dans l?ordre du fichier, jusqu?? cinq par page. Les grilles inutilis?es sur la derni?re page restent vides. **150 jeux produisent 30 pages.**

## Param?tres d?impression

- **Taille r?elle / ?chelle : 100 %.**
- **Sans ajustement ? la page.**
- **Format papier personnalis? : largeur 160 mm ? hauteur 152 mm.**
- Sans agrandissement sans bordure et sans recto verso.
- Une page PDF par bulletin ; respecter le sens d?insertion.

Le PDF conserve le format initial de calibrage **160 ? 149 mm**. Le format papier **160 ? 152 mm** est le r?glage rapport? comme satisfaisant par Math06 lors du test de calibrage.

Les tirages et le nombre de samedis sont ? cocher manuellement sur les bulletins. Cette premi?re version est destin?e aux essais : l?alignement et la r?p?tabilit? de l?impression en s?rie restent ? confirmer sur les bulletins r?els.

## Licence

[Apache License 2.0](LICENSE).

Projet ind?pendant, sans partenariat ?tabli avec FDJ ou le groupement ? nous les millions.
