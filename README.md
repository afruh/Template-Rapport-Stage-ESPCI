# Template-Rapport-Stage-ESPCI
Un modèle de rapport pour les différents stages de l'ESPCI.

## Installation
1. Il faut créer un nouveau projet puis choisir Upload Project, déposer le fichier `Template ESPCI - Stage.zip`.
2. Il va y avoir des erreurs de compilation car il faut utiliser le Compilateur `XeLaTex`. Pour cela il faut cliquer sur Menu (en haut à gauche de l'interface). Dans la fenêtre qui vient de s'ouvrir , il faut changer Compiler via le menu déroulant en choisissant `XeLaTeX`.

## Description
Template réalisé par Arthur Fruh 139 pour les différents rapport de stage (1A, ingénieur P3A) pour l'ESPCI
Si jamais vous vouler utiliser la police cera il suffit de taper `\cera` ( elle est compatible avec `\textbf{}` ).
la couleur bleue utilisée par la charte graphique est utilisable en utilisant `\color{pantone281}`.
`sources.bib` permet de gérer la bibliographie et d'utiliser la commande `\cite{référence_article}` pour citer une référence.

## Modifier la police
Pour remettre la police du corps de texte comme initialement dans Latex: il sufit de commenter la commande `\usepackage{CormorantGaramond}` dans les premières lignes de `main.tex`.

Pour les titres il faut : 
1. Il suffit de changer les fichiers `.otf` et mettre vos fichiers de polices.
2. Il faut reporter les modifications dans `config/settings.tex` ligne 29. Changer l'extension si nécessaire et les autres paramètres en fonctions des polices importer ( BoldFont permet d'utiliser la commande `\textbf{}` ). ATTENTION : laisser le même nom pour la commande `\cera`, sinon il faudra changer le reste du fichier.

## Filigrane (Confidentiel par exemple)
Il faut décommenter les lignes 11 à 15 du fichier main.tex, puis les modifier comme bon vous semble. N'hésitez pas à regarder la docmentation du package draftwatermark
