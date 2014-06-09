anim_newbie
===========

Quelques animations "test" réalisées dans le cadre d'un cours d'initiation à l'animation pour le web.

Comment ça marche
-----------------

Ces animations ont été développées dans un cours d'initiation à l'animation pour le web.

Pour utiliser ces animations :

1. télécharger la feuille de style "anim_newbie.css" et l'enregistrer dans le répertoire de votre projet web.

2. attacher la feuille de style "anim_newbie.css" à l'intérieur des balises "head" de votre page web 

3. ajouter la classe d'animation désirée à l'élément que vous souhaitez animer : arrivee_deployee, balance, degringolade, bondissant ou pulsation.

Les animations sont conçues pour s'exécuter sur des éléments en mode "display:block" ou "display:inline-block". Les animations fonctionneront mal (ou pas du tout) sur des éléments en mode "display:inline".

Pour de meilleurs résultats, l'animation "degringolade" doit être appliquée à un objet centré horizontalement et placé en haut de la page.



Personnaliser l'animation
-------------------------

Par défaut, chaque animation ne s'exécute qu'une seule fois. Pour que l'animation joue de façon infinie, il suffit d'ajouter la classe "animation-infinite" à l'objet animé. À noter que l'animation infinie n'est pas recommandée pour les animations "arrivee_deployee" et "degringolade". 

On peut aussi personnaliser le nombre de fois que l'animation s'exécute, sa durée, ou encore prévoir un délai avant son exécution en ajoutant à l'élément animé un ID contenant, dans la feuille de style CSS, les informations suivantes :

* Pour changer le nombre de fois que l'animation s'exécute :
```
animation-iteration-count: 1;
-webkit-animation-iteration-count: 1;
-moz-animation-iteration-count: 1;
-ms-animation-iteration-count: 1;
-o-animation-iteration-count: 1;
```
  Sur chaque ligne, remplacer le "1" par le nombre de fois que vous souhaitez voir l'animation se répéter.

* Pour changer la durée :
```
animation-duration:2s;
-webkit-animation-duration:2s;
-moz-animation-duration:2s;
-ms-animation-duration:2s;
-o-animation-duration:2s;
```
  Sur chaque ligne, remplacer le "2s" par la durée désirée. Elle peut être définie en secondes (en spécifiant "s" comme unité) ou en millisecondes (en spécifiant "ms" comme unité). Si aucune unité n'est définie, l'utilisation des secondes est supposée.

* Pour ajouter un délai avant l'exécution de l'animation :
```
animation-delay: 2s;
-webkit-animation-delay: 2s;
-moz-animation-delay: 2s;
-ms-animation-delay: 2s;
-o-animation-delay: 2s;
```
  Sur chaque ligne, remplacer le "2s" par le délai désiré. Il peut être défini en secondes (en spécifiant "s" comme unité) ou en millisecondes (en spécifiant "ms" comme unité). Si aucune unité n'est définie, l'utilisation des secondes est supposée.

Toutes ces modifications doivent être ajoutées dans le même ID si vous souhaitez modifier plus d'une propriété.
