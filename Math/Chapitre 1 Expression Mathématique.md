[[MT02]]

#tags: #math #logique #proposition #todo
Voir aussi : [[Ensembles]] | [[MT03]]

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

*Bon à partir de là j'ai la flemme de tout taper

## Implication
$$
(P \implies Q) \leftrightarrow (\neg P\wedge Q)
$$

$$
\neg(P\implies Q) \leftrightarrow (P \vee \neg Q)
$$

#demo

En comparant les tableaux de vérités, on peut conclure que les deux propositions sont équivalentes
Pour la deuxième, il suffit de distribuer le NON.

#correction
Soit $f(R)\to R$
Nier les propositions suivantes
1) P1 "Le graphe de f coupe la droite d'équation y = x au moins en un point"
2) P2 "f est la fonction nulle"

Réponses :
1) $\forall x \in R,f(x)\neq x$
2) $\exists x \in R,x\neq 0$

$$
n^{2} pair \implies npair

$$
par l'absurde, on suppose que n^2 pair ET n impair :
$$
n^{2}=2k
$$$$
n = 2k' +1
$$
$$
n^{2}+n=n(n+1) \implies pair
$$
$$
\leftrightarrow 2(k + k') + 1 \implies impair??
$$
On vient de trouver une contradiction, donc la proposition est vraie

On peut le faire plus facilement avec la contraposée (n impair) -> (n^2 impair)

# Récurrence

Si une proposition dépend de n entier naturel
$$
P(n), \forall n\geq n_{0}, n_{0}\in N
$$ ... est vrai par récurrence

1) initialisation
	1) $P(n_{0})$ est vrai
2) hérédité
	1) $P(n)\implies P(n+1)$ est vrai
3) conclure que $P(n), \forall n\in N$ est vrai

Exemple:
$\forall n \geq 1$
$$
\sum_{k=1}^{n}k = \frac{n(n+1)}{2}
$$
Init :
P(1)
$$
\sum_{k=1}^{1}k = 1 
$$
... vrai

Heredité :
on suppose P(n), on montre que $P(n)\implies P(n+1)$

$$
\sum_{k=1}^{n+1} k = (\sum_{k=1}^{n} k) + (n+1)
$$$$
\implies \frac{n(n+1)}{2} +n+1
$$$$
\implies \frac{(n+1)(n+1)}{2} \leftrightarrow  \sum_{k=1}^{n+1} 
$$
L'hérédité est vérif

Conclusion :
Comme $P(1)$ vrai et $P(n)\implies P(n+1)$, alors $P(n)$ vrai $\forall n \in N*$
