# Latex

base pour les documents latex,

## Creer un document :
dans le dossier tex, créer votre fichier *nomDuFichier.tex*, dans le fichier *main.tex* ajoutez la ligne *\input{nomDuFichier}*, puis compilez.

## Compilation :
La compilation se fait simplement en utilisant le script *latexBuild*

```Shell
> ./latexBuild -f tex/main.tex
```

## Arborescence :
- tous les fichiers *tex* / *bib* sont placés dans un sous dossier *tex*
- toues les images sont placés dans un dossiers *res*, elles seront automatiquement converties en *eps* puis déplacés vers *used*

les *\input{}* et *\includegraphics{}* se font en faisant référence au dossier d’où est lancé la commande *latexBuild*

```Shell
.
├── tex
│   ├── main.bib
│   ├── ...
│   └── main.tex
├── res
│   ├── image1.png
│   ├── ...
│   └── image2.jpg
├── _minted
│   ├── ...
│   └── ...
├── README.md
└── used

```
