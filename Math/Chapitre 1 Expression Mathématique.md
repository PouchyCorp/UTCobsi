[[MT02]]

[[MT02-ch1_ecran.pdf]]

1 - Toute proposition a une valeur de vérité

#exemple 
"Soit x un réel, alors x > 0" Faux
"Tout x réel positif est supérieur ou égal à zero." Vrai
"x est supérieur ou égale à zero" Proposition invalide
# I - Logique

#definition 
Un énoncé mathématique affirme une ou plusieurs propriétés, dans un domaine donné.
La logique permet d'attribuer une **valeur de vérité** 
### Trois principes logique:
- Le principe d'identité : $P = P$
- Le principe de non-contradiction: *Si $P$ est vrai, alors $P$ n'est pas faux.
- Le principe du tier exclu : *Les seuls états possible de $P$ sont Vrai ou Faux

#definition
Axiome : Vérité absolue, tout raisonnement logique s'appuie sur eux.

#exemple 
Axiome de Peano : *Si une partie $P$ de $N$ contenant $0$ tel que le successeur de chaque élément de $P$ est dans $P$, alors $P=N$.* (Principe de la récurrence)

#definition 
Théorème : Une proposition dont on démontre la véracité 
Corollaire : Une conséquence du théorème
Lemme : Une propriété importante pour démontrer un théorème 

# II - Le vif du sujet
## A - Négation
On note "NON $P$" ou "$\neg P$"
Nier $P$, c'est passer la définition de l'ensemble de $P$ à son ensemble **complémentaire**

Si $P$ Vrai, alors $\neg P$ Faux.
## B - Conjonction
Noté "ET" ou "$\wedge$"

#exemple 
$P$ : n entier pair
$Q$ : n multiple de 3
$P\wedge Q$ : n multiple de 6

## C - Disjonction
Noté "OU" ou "$\vee$"

$P\vee Q$ Faux ssi $P$ Faux et $Q$ Faux.

## D - Equivalence
On note "equivalent", "si et seulement si (ssi)", "$\leftrightarrow$" ou bien encore "$\equiv$"

$P \leftrightarrow Q$ vrai ssi $P$ et $Q$ sont tout les deux vrai ou faux, ils sont **CNS (Condition Necessaire et Suffisante)**

#exercice 
$P$ : $n \geq 3$ et $n$ premier
$Q$ : $n$ impair
$$
P \leftrightarrow Q ?
$$
Non,
puisque il ne suffit pas que $n$ soit impair pour que il soit premier ou supérieur à trois.
Donc
$$
P\implies Q
$$$$
Q \nRightarrow P
$$

