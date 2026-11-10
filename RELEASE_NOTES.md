# Notes de version — CrescendoPrinter

Copyright © 2026 Claude Lalyre

## 0.0.1 — 10 novembre 2026

Première version de l’application Windows destinée aux essais d’impression en série avec Math06.

### Fonctionnalités

- Chargement d’un fichier texte : un jeu de 10 numéros distincts entre 1 et 25 par ligne, séparés par des espaces, des points-virgules ou des tirets.
- Prise en charge des fichiers UTF-8 avec ou sans BOM et Windows-1252 ; lignes vides ignorées.
- Validation du fichier complet, avec une fenêtre d’erreur indiquant le numéro de la ligne invalide.
- Génération d’un PDF avec jusqu’à cinq jeux par page, dans l’ordre du fichier, et pagination des bulletins.
- Grilles inutilisées de la dernière page laissées vides ; 150 jeux produisent 30 pages.
- Rappel des paramètres d’impression dans la fenêtre.
- Binaire autonome `CrescendoPrinter.exe`, construit avec Python 3.13 dans `venv13` et PyInstaller via `build_exe.bat`.
- Version affichée dans le titre de la fenêtre et dans les propriétés du binaire Windows.

### Réglages d’impression

- Taille réelle / échelle **100 %**, sans ajustement à la page.
- Format papier personnalisé : **160 mm de large × 152 mm de haut**, suivant le retour de Math06 sur le calibrage.
- Sans agrandissement sans bordure et sans recto verso.
- Le PDF conserve le format initial **160 × 149 mm** et les coordonnées du calibrage.

### Limites et validation

- L’impression se fait depuis un lecteur PDF après génération du document.
- Les tirages et le nombre de samedis sont à cocher manuellement sur les bulletins.
- Les tests automatisés couvrent la validation des jeux, le chargement dans l’interface et les PDF multipages, dont un lot de 150 jeux.
- L’essai de cette application sur de vrais bulletins reste à réaliser avec Math06 pour confirmer l’alignement et la répétabilité de l’impression en série.
