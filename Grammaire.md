	
**Dérivation**: Une dérivation en analyse syntaxique est une façon de d'attribuer une règle à un non terminaux.

**Exemple**:
	Pour un set V de non terminaux.
	$\text{V =}$ $\set{E, X, D}$
	$\text{E -> X | E}$
	$\text{X -> D + E}$
	$\text{D -> Number}$
	Etant donnée un set V nous dérivons chaque non terminal par des règles.
	
	
	
**Axiome de depart:** L'axiome de départ S est un non-terminal c'est le premier non-terminal qui va être dérivé.



**Non terminaux:** C'est un ensemble V de valeur litteraux qui peuvent avoir plusieurs règle.



**Exemple:**
	$\text{V =}$ $\set{E}$
	En effet l'on peut voir que l'on obtient un set de non terminaux.
	$\text{E -> XE}$
	$\text{E -> EX}$
	En effet comme vous pouvez le voir nous avons appliqué plusieurs règle à même non Terminal.



**Terminaux:** C'est un ensemble de valeur litteraux qui ont une valeur fixe.



**Exemple:**
	$\text{V =}$ $\set{E}$
	$\text{A =}$ $\set{number, (, ), +}$
	$\text{E -> number}$
	$\text{E -> E+E}$
	$\text{E -> (E)}$
	En effet number est un terminal étant donné qu'il ne peut être dérivé.
	
	

**Alphabet:** A est un ensemble de terminaux, utilisé dans les règles.




**Exemple:**
	$\text{A =}$ $\set{number, (, ), +}$
	
	

**Exemple règle arithmétique:**
	$\text{A =}$ $\set{number, (, ), +}$
	$\text{V =}$ $\set{E}$
Règle:
E -> number
E -> (E)
E -> E+E
E -> E/E
E -> E-E
Ou:
E -> number
    | (E)
    | E+E
    | E/E
    | E-E
			    
			    
Prenons à présent une opération arithmétique et regardons si celle-ci est conforme à notre règle syntaxique.

$\text{2+5 / (3+6)}$
Linéaire représentation:
$\text{E -> E+E -> E/E -> E / (E) -> E+E -> E+E / (E+E)}$
number + number / (number + number)
Nous avons donc dérivé notre opération de manière linéaire.

	

Epsilon: c'est simplement lorsque la dérivation est vide.

Arbre de dérivation:

Une dérivation enchainant plusieurs dérivation peut se représenter sous forme d'arbre. On appelle ça un arbre de dérivation. Le noeud root correspond à l'axiome, les autres noeud sont les non-terminaux et les feuilles sont les terminaux. Lorsqu'un non-terminal n'a pas de terminal on lui met une feuille  $\epsilon$

$\text{E -> E * E -> E * (E) -> E * (E + E)}$
Exemple:

				![[Pasted image 20230210170928.png]]
