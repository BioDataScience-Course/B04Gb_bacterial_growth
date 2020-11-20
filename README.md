La croissance bactérienne
================

## Avant-propos

Les consignes sont reprises dans ce document, ainsi que sous forme de
commentaires dans les différents fichiers. Elles sont susceptibles
d’évoluer. N’hésitez pas à vérifier le lien suivant afin de voir si
des modifications n’y ont pas été apportées :
<https://github.com/BioDataScience-Course/B04Gb_bacterial_growth>

## Contexte

Des scientifiques ont réalisé une culture bactérienne et tentent de la
modéliser. Malheureusement, ceux-ci n’ont pas vos connaissances et ils
vous demandent de les aider à modéliser les données qu’ils ont obtenues.

A partir de leurs données (`growth_curve.tsv`) disponiblent dans le
dossier `data`, le graphique suivant peut-être réalisé.

``` r
bacteria <- read("data/growth_curve.tsv")
```

    ## Parsed with column specification:
    ## cols(
    ##   time = col_double(),
    ##   growth_log = col_double()
    ## )

``` r
chart(bacteria, growth_log ~ time) +
  geom_point()
```

![](README_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

## Objectif

Ce projet est un projet **individuel**, **court** et **libre** qui doit
être **terminé pour la fin du module 4**.

Complétez le cahier de laboratoire (`bacterie_notebook.Rmd`) présent
dans le dossier `docs` en réalisant trois modèles non linéaire pour
essayer de modéliser la croissance bactérienne.

Sélectionnez le meilleur modèle et justifiez votre choix.
