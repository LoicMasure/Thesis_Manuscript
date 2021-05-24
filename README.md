# Thesis Manuscript
## Loïc Masure - December, 18 2020 (oral defense)
This repository contains all the source files required to compile my thesis manuscript. I make it available online so that it may help any PhD student to start with a template. I started myself with a template from the Dorian Depriester's [blog post](https://blog.dorian-depriester.fr/latex/template-these/template-complet-pour-manuscrit-de-these), and transcripted it in english.

This work is also made available to the Side-Channel Analysis community to better seed my work, while waiting for my university to publish my manuscript.

### Reproduction
You are free to reproduce or take inspiration from the texts without asking permission, provided that you comply with the original work's license (see link above) and that you cite this work.

Concerning reproducing figures, please ask permission to me (loic.masure@hotmail.fr) or directly to the figures' owner if I reproduced myself a figure (see the the owner's name in the figure's legend).


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
