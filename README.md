# _ObserverPattern_

#_Description_

 Ce exemple concerne une classe diffuseuse d'événement(Editor, bouton), une Interface souscripteur(écouteur) qui définie les différents souscripteurs  avec la possibilité d'être ajouter comme écouteur au niveau de la classe diffuseuse(editor, bouton).. ,une classe Gestion des événements qui permet de gérer les événement et considérer comme étant l'interface a travers laquelle la classe diffuseuse communiquera avec la classe souscriptrice.
Avec ce type d'exemple il serait plus simple de séparer les classes afin d'avoir une classe de gestion des événements centralisé.  

-Identification : Ce patron peut être reconnu <<dans les méthodes de souscription qui stockent des objets dans une liste>> et par <<les appels des objets de cette liste à la méthode update>>. 

Nb:  chaque événement(opération) ne doit concerné que l'ensemble des objets qui lui sont associé. Il faut pas qu'un événement (open) par exemple ait un impacte su tout les éléments. 
Un événement doit être limité a la liste d'éléments qui le concerne.

-Ainsi avec ce design pattern le fait que les classes ne soit pas couplet cela permet de les réutilisées dans d'autre application.
-Nous pouvons également ajouter d'autre type de fonctionnalité(d'autre classe écouteur, souscripteurs) sans pour autant modifié le code de Editor/bouton
 
