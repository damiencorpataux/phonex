# phonex

Algorithme **phonex** pour **python3**
* porté par [Ophir LOJKINE](https://github.com/lovasoa/phonex)
* écrit par [Frédéric BROUARD](http://info.univ-lemans.fr/~carlier/recherche/soundex.html)
* packagé pour `pip` par [Damien CORPATAUX](https://github.com/damiencorpataux/phonex)

Installation
-
```
pip install phonex
```

Usage
-
La fonction `phonex` retourne un nombre qui correspond à la prononciation d'un mot en français.

```
>>> from phonex import phonex
>>> phonex('Dupont')
0.7638993238166792
>>> phonex('Dupond')
0.7638993238166792
>>> phonex('Clairac')
0.47921338864425217
>>> phonex('Clairaque')
0.47921339555074816
```

Crédits
-
> Phonex est un algorithme de Soundex plus perfectionné [...] que la version francisée de Soundex2.
Sachez que Phonex est optimisée pour le langage français, sait reconnaître différents types de sons
comme les sons ‘on’, ‘ai’, ‘ein’, etc... et place son résultat sous la forme d’un réel de type double précision
(5.0 x 10-324 .. 1.7 x 10308 sur 15 à 16 chiffres significatifs).
Son temps de calcul est double de Soundex et 30% supérieure seulement à Soundex2.

Algorithme Phonex,
Copyright Frédéric BROUARD (31/3/99),
[Voir la version originale](http://info.univ-lemans.fr/~carlier/recherche/soundex.html).