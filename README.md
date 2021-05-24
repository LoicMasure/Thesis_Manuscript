# Manuscrit de thèse
## Loïc Masure - 2020
This repository contains all the source files required to compile my thesis manuscript. I make it available online so that it may help any PhD student to start with a template. I started myself with a template from the Dorian Depriester's [blog post](https://blog.dorian-depriester.fr/latex/template-these/template-complet-pour-manuscrit-de-these), and transcripted it in english.

### Reproduction
You are free to reproduce or take inspiration from the texts without asking permission, provided that you cite this work as follows.
```
```
Concerning reproducing figures, please ask permission to me (loic.masure@hotmail.fr) or directly to the figures' owner if I reproduced myself a figure (see the the owner's name in the figure's legend).

### Structure

* Cover Page
* Table of Contents

1. Chapter 1
  * Epigraph
  * Mini table of contents
  * Body
2. Chapitre 2
  * Idem
3. Etc.

* Appendices :
  * Appendix A
  * Etc.
  * Acronyms
  * Symbols
  * Glossary
* List of figures
* Liste of tables

## Compilation
````bash
pdflatex Main
bibtex Main
makeglossaries Main
pdflatex Main
pdflatex Main
````


## Writing chapter-wise
In the ``Main.tex`` file, one must add the following line to define the list of chapters to compile:
````latex
\includeonly{Chapitre1,Chapitre2,Annexes}
````

## Glossary
The glossary entries are defined in ``Glossary.tex``. To call one glossary entry, use the following line:
````latex
\gls{<label>}
````
The [documentation](http://tug.ctan.org/tex-archive/macros/latex/contrib/glossaries/glossaries-user.pdf) of the ``glossaries`` Latex package may help.
