--- 
title: Documentation
bookToc: false
categories: [
    "Go",
]
tags: [
    "templates",
    "programmation",
    ]
---

## Ressources

Cette page référence les documentations utiles au cours sur l'usage des outils. 

Index : 

- [Hypothesis](https://mmellet.github.io/ELD718/documentation/#hypothesis)
- [Github](https://mmellet.github.io/ELD718/documentation/#github)
- [Leaf-Writer](https://mmellet.github.io/ELD718/documentation/#leaf-writer)
- [Markdown](https://mmellet.github.io/ELD718/documentation/#markdown)
- [Pandoc](https://mmellet.github.io/ELD718/documentation/#pandoc)
- [Raccourcis clavier](https://mmellet.github.io/ELD718/documentation/#raccourcis-clavier)
- [Scribus](https://mmellet.github.io/ELD718/documentation/#scribus)
- [Stylo](https://mmellet.github.io/ELD718/documentation/#stylo)
- [Zotero](https://mmellet.github.io/ELD718/documentation/#zotero)


-------------------------

### Raccourcis clavier 

#### Gestion Écriture
- CTRL/Cmd + C : Copier (*Copy*)
- CTRL/Cmd + V : Coller (*Varnish*)
- CTRL/Cmd + X : Couper (*eXterminate*)

- CTRL/Cmd + A : Sélectionner tout (*All*)
- CTRL/Cmd + F : Rechercher (*Find*)

- CTRL/Cmd + Z : Annuler (*Zut*)
- CTRL/Cmd + Y : Revenir à l'état précédent (*Yesterday*)

#### Gestion Document
- CTRL/Cmd + S : Sauvegarder (*Save*)
- CTRL/Cmd + O : Ouvrir (*Open*)
- CTRL/Cmd + Q : Quitter (*Quit*)
- CTRL/Cmd + N : Nouvelle fenêtre (*New*)
#### Traitement texte 
- CTRL/Cmd + B : Mise en gras (*Bold*)
- CTRL/Cmd + I : Mise en italique (*Italique*)
- CTRL/Cmd + U : Souligner (*Underline*)

-------------------------
-------------------------

### Hypothesis 

- [Astuces pour des annotations réussies](https://web.hypothes.is/annotation-tips-for-students/)

-------------------------
-------------------------
### Zotero

[Atelier](https://mmellet.github.io/ELD718/slides/Seance-2.html#/6)

-------------------------
-------------------------
### Scribus

- [Atelier 1](https://mmellet.github.io/ELD718/slides/Seance-2.html#/6)

- [Atelier 2](https://mmellet.github.io/ELD718/slides/Seance-3.html#/5)
    - Exemple de résultat : [PDF](https://mmellet.github.io/ELD718/doc/Atelier-Scribus.pdf) et [.sla](https://mmellet.github.io/ELD718/doc/Atelier-Scribus.sla)
#### Raccourcis Scribus

Aide : F1
Panneau Propriété : F2

##### Actions sur un élément 
- E : Editer le contenu (texte pour un bloc de texte)
- N : Lier les cadres de texte
- Ctrl+A : Sélectionner tout
- Ctrl+C : Copier
- Ctrl+D : Dupliquer
- Ctrl+F : Rechercher-Remplacer
- Ctrl+S : Enregistrer

##### Ajouter des éléments 
- B : Tableau 
- I : Bloc Image 
- T : Bloc Texte 
- I : Bloc Image 

[Plus de raccourcis encore](https://wiki.scribus.net/canvas/Raccourcis_clavier,_par_touche)

-------------------------
-------------------------

## Stylo

- [Atelier 1](https://mmellet.github.io/ELD718/slides/Seance-4.html#/4)
- [Atelier 2](https://mmellet.github.io/ELD718/slides/Seance-5.html#/5)


-------------------------
-------------------------

## Pandoc 

- [Atelier](https://mmellet.github.io/ELD718/slides/Seance-6.html#/6)

### Commandes Terminal 

#### Navigation 

| Action  | Linux/MacOs  | Windows |
|---|---|---|
| où je suis  | `pwd` (*Print Working Directory*) | `cd` (*Current Directory*) |
| aller/ se deplacer  |  `cd chemin` (*Change Directory*) | `cd chemin` (*Change Directory*) |
| revenir en arrière  |  `cd ..`   | `cd ..` |
| lister les fichiers (avec meta information) |  `ls -l` ou `ll`  | `dir` |
| recherche dans les noms des fichiers |  `find ~ -name '*.md'` | `dir -s  *.md` |
| recherche dans les contenus des fichiers |  `grep site README.txt` | `findstr site .\README.md` (cherche le mot `site` dans le ficher `README.md` ) |

#### Gestion des fichiers

| Action  | Linux/MacOs  | Windows |
|---|---|---|
| déplacer un fichier (ex: deplacer fichier dans dossier parent) | `mv README.md ../`(*Move*) | `move README.md ../`  |
| supprimer un fichier | `rm README.md` (*Remove*) |`del README.md` (*Delete*)|
| afficher le contenu |`cat README.md` (*Concatenate*)| `gc README.md` (*Get-Content*) |
| créer un fichier vide | `touch README.md` ou `echo '' >> README.md` | `echo $null >> README.md` |
| créer un dossier | `mkdir newFolder` (*Make Dir*) | `mkdir newFolder` (*Make Dir*)  |
| supprimer un dossier vide | `rmdir newFolder` (*Remove dir*) | `rmdir newFolder` (*Remove dir*)  |
| copier un fichier | `cp README.md README2.md` (*Copy*) | `copy .\README.md .\README2.md`|
| copier un dossier | `cp -r content content2` (*Copy recursively*) | `Copy-Item -Path content -Destination content2 -Recurse`|

#### Astuces 

- tabulation : autocomplétion
- flèche du haut : historique des commandes
- CTRL + R : rechercher dans l’historique

- `clear` pour effacer les commandes affichées

- `&&` pour enchaîner les commandes
  - ex: ` echo "Hello!" && echo "World!"`
- `wc nom.extension` pour compter les noms (*WordCounter*)

--------------------
------------------

### Github

- [Atelier Github](https://mmellet.github.io/ELD718/slides/Seance-7.html#/5)

### Leaf-Writer

- [Atelier Leaf-Writer](https://mmellet.github.io/ELD718/slides/Seance-8.html#/4)

<!--
## Commandes Bash


- pour générer du texte : 

        echo "texte" ;

-----

- pour afficher le contenu d'une valeur : 

        texte='je suis une chose';
        echo ${texte}
        
PS : *Attention à ne pas insérer d'espace avant ou après le "=" de la valeur.*

----

- pour afficher le contenu d'une valeur dans du texte : 

        texte='je suis une chose';
        echo "je déclare que : ${texte}"
    

- pour générer du texte interactif : 

        read p 'Entrez votre nom : ' nom
        echo "Bonjour $nom !"
        
        
-----

- pour introduire une commande : 

        horaire=`date`
        echo "Aujourd'hui EST $horaire"

PS : *Ici la valeur "horaire" est une commande qui affiche le date*.

- autre exemple : 

        prison=`pwd`
        echo "Vous êtes coincé dans le dossier $prison"

PS: *pwd permet de savoir où je me trouve dans ma machine*.

----

- pour insérer des latences : 

        sleep *temps* ;

*soit pour une pause de 0,3 secondes, je note :* 
    
        sleep 0.3 ; 

----

- pour demander mon identité : 

        whoami; 

*étant donné que vous êtes sur une interface en ligne, il ne vous donnera aucune identité*

----

- pour ajouter une identité : 

        useradd
        
    ou la supprimer : 
    
        userrm

*de même ces commandes vont vous être refusées*

-----

- pour générer du texte inarrêtable : 

        yes "texte";

----

- pour effacer les écritures précédentes : 

        clear

----

- composer un programme d'écriture : 

        T[0]='texte1'
        T[1]='texte2'

        echo ${T[0]} ${T[1]}
    ou 

        T[0]='texte1'
        T[1]='texte2'

        echo ${T[*]}
        

----

- insérer des coupes : 

       T[0]='texte non coupé'

        echo ${T[0]}| cut -c1-5,9-15

--- 

- renverser l'écriture : 

        echo "Hello World" | rev


----


- script pour créer de l'interaction avec mon lecteur : 
    
        echo "Etes vous humain ou machine ?"
            select i in humain machine; do
                if [ "$i" = "humain" ]; then
                    echo "Bonjour";
                    sleep 0.9;
                    echo "soyons amis";
                    break
                elif [ "$i" = "machine" ]; then
                    echo "Bonjour camarade"
                    sleep 0.9;
                    echo "veux-tu m'aider à détruire les humains?"
                    break
                else
                    echo "je ne peux vous identifier"
                fi
        done

-----

- script enchâssé : 

                echo "Etes vous humain ou machine ?"
            select i in humain machine; do
                if [ "$i" = "humain" ]; then
                    echo "l'êtes vous vraiment ?";
                        select i in oui non; do
                            if [ "$i" = "oui" ]; then
                                echo "si vous êtiez humain vous douteriez... doutez-vous?";
                                    select i in oui non; do
                                        if [ "$i" = "oui" ]; then
                                            sleep 0.9;
                                            echo "alors bienvenu humain qui doute";
                                            break
                                        elif [ "$i" = "non" ]; then
                                            echo "Vous n'êtes pas honņête"
                                             sleep 0.9;
                                            echo "je vous exclu de cet espace"
                                            sleep 0.9;
                                            break
                                        else
                                        echo "la question était pourtant sans équivoque"
                                        fi
                                    done
                            elif [ "$i" = "non" ]; then
                                echo "je le savais"
                                sleep 0.9;
                                echo "bonjour machine qui veut être humain"
                                break
                            else
                                echo "vous ne coorpérez pas"
                            fi
                        done
                elif [ "$i" = "machine" ]; then
                    echo "Bonjour camarade"
                    sleep 0.9;
                    echo "veux-tu m'aider à détruire les humains?"
                    break
                else
                    echo "je ne peux vous identifier"
                fi
            done


----

- texte inarrêtable horizontal : 

        while true; 
       do printf "texte" $((RANDOM%1));
             for ((i=-0; i<$((RANDOM%128)); i++))
                   do printf " ";
                   done;
        sleep 0.2;

       done;

-------------
----------

### Zotero 

<iframe src="https://mmellet.github.io/FRA3826_2023/slides/Zotero.html" title="description" height="500" width="800" ></iframe>

<div style="text-align:center">
<a href="https://mmellet.github.io/FRA3826_2023/slides/Zotero.html" target="_blank">ouvrir dans mon navigateur</a>
</div>

-------------------------
-------------------------

<!--
## HedgeDoc 

[HedgeDoc](https://docs.hedgedoc.org/) est un espace pour l'écriture collaborative et synchrone. 

 
Cet espace se structure selon 2 espaces :

![](/images/hedge.png)

### ![](/images/writing.png) Espace d'édition 

![](/images/exwriting.png)

C'est dans cet espace que vous pourrez éditer. 

L'édition d'une note peut être effectuée via l'éditeur visuel :

![](/images/editor.png)

ou directement en Markdown dans le texte.


### ![](/images/visual.png) Espace de visualisation 

![](/images/exvisual.png)

Cet espace n'est pas éditable mais permet un rendu type web. 

### ![](/images/double.png) Double configuration

![](/images/exemple.png)

Afin de suivre en simultané le rendu de votre édition vous pouvez choisir la double configuration. 


### [Index des notes collaboratives](https://demo.hedgedoc.org/sl_ISH8hSDSCQ9TUQEDzQg?both)

L'index pour les prises de notes collaboratives se trouve [ici](https://demo.hedgedoc.org/sl_ISH8hSDSCQ9TUQEDzQg#).

-------------------------
-------------------------
-->

### Markdown

Markdown est un langage sémantique. 

Voici les fondamentaux : 

#### Niveaux de titre 

Les niveaux de titre se notent avec l'utilisation du dièse : 

```

## Titre de niveau 2 

### Titre de niveau 3 

```

#### Italique et gras

```
- *italique*
- **gras** 
- ***gras italique***

```

#### Notes 

```
Voici mon texte^[une note de bas de page inline.]

Voici mon texte[^1] 

[^1]:Une note de bas de page avec appel et renvoi

```

#### Liens

```
[un lien vers une page Wikipédia](https://fr.wikipedia.org/wiki/Hyperlien)

```
 
#### Image

```
![Légende](https://tonpetitlook.com/wp-content/uploads/2017/05/nouveau-chaton-nouveau-defi-430442.png)
```

#### Tutoriel

<a href="https://www.arthurperret.fr/tutomd/" target="blank">Traduction en ligne par Arthur Perret</a>
					
<!--
-------------------------
-------------------------


### HedgeDoc 

[HedgeDoc](https://docs.hedgedoc.org/) est un espace pour l'écriture collaborative et synchrone. 

 
Cet espace se structure selon 2 espaces :

![](https://mmellet.github.io/FRA3826_2023/images/hedge.png)

#### ![](https://mmellet.github.io/FRA3826_2023/images/writing.png) Espace d'édition 

![](https://mmellet.github.io/FRA3826_2023/images/edition.png)

C'est dans cet espace que vous pourrez éditer. 

L'édition d'une note peut être effectuée via l'éditeur visuel :

![](https://mmellet.github.io/FRA3826_2023/images/editor.png)

ou directement en Markdown dans le texte.


#### ![](https://mmellet.github.io/FRA3826_2023/images/visual.png) Espace de visualisation 

![](https://mmellet.github.io/FRA3826_2023/images/visualisation.png)

Cet espace n'est pas éditable mais permet un rendu type web. 

#### ![](https://mmellet.github.io/FRA3826_2023/images/double.png) Double configuration

![](https://mmellet.github.io/FRA3826_2023/images/dual.png)

Afin de suivre en simultané le rendu de votre édition vous pouvez choisir la double configuration. 


-------------------------
-------------------------



------------------
---------------------
