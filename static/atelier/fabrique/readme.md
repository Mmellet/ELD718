
Prérequis : [installer pandoc](https://pandoc.org/installing.html)

## Pour la conversion vers ePub

Taper ou Copier/Coller dans votre terminal : 

```
pandoc --citeproc -f markdown -t epub texte.md -o texte.epub
```

## Pour la conversion vers DOCX : 

Taper ou Copier/Coller dans votre terminal : 

```
pandoc --citeproc -f markdown -t docx texte.md -o texte.docx
```

--- 

## Pour la conversion vers HTML : 

Taper ou Copier/Coller dans votre terminal : 

```
pandoc --citeproc --template=templateHTML.html5 -f markdown -t html5 texte.md -o texte.html
```

---- 

---- 



## Pour la conversion vers PDF :

Prérequis : 

Windows et Mac : 
[installer MiKTeX](https://miktex.org/download)


Taper ou Copier/Coller dans votre terminal : 

```
pandoc --citeproc -f markdown -t pdf texte.md -o texte.pdf
```

### Personnaliser son PDF : utiliser un template 

Taper ou Copier/Coller dans votre terminal : 


```
xelatex texte2.tex 

```

L'étape préliminaire (que vous n'avez pas à faire) : 

```

pandoc --citeproc --csl=apa.csl --template=templatePDF.latex -f markdown -t latex texte.md -o texte2.tex

``` 