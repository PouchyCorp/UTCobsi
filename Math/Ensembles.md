[[MT02]]

#tags: #math #ensembles #logique #todo
Voir aussi : [[Chapitre 1 Expression Mathématique]] | [[MT03]]

### Bases

#definition 
On appelle ensemble noté $E$ une collection d'objets ayant une ou des propriétés communes
On appelle les objets "élément" de $E$
Un élément $x$ apparient à $E$ et écrit $x \in E$

#definition
L'ensemble vide est noté $\varnothing$

#definition 
Soit $E$ un ensemble et $A$ une partie de $E$
on dit que $A$ est un sous ensemble de $E$
noté $A \subset E$ on lit "A inclut dans E"
$$
(A \subset E) \leftrightarrow (\forall a \in A, (a \in E) \vee (A = \varnothing))
$$
Donc, $$
\forall E, \varnothing \subset E
$$
#exemple $$
N \subset Z \subset A \subset R \subset C
$$$$
R^+ \subset R
$$
Pour montrer que $A \not\subset E$, il faut montrer:
$$
\neg(\forall a \in A, a \in E) \leftrightarrow (\exists a \in A, a \not\in E)
$$

### Complémentaire
#definition 
Soit $A \subset E$, on appelle complémentaire de A dans E le sous-ensemble de E défini par :
$$
\neg(a \in A, a \in E) \leftrightarrow  (a \not\in A, a \in E)
$$
$$
\complement_{E}E = \varnothing
$$$$
\complement_{\complement_{E}E}E = E
$$$$
\complement_{\varnothing}E = E
$$
#proposition$$
(A = B) \leftrightarrow (A \subset B \wedge B \subset A)
$$
#todo : Prouver que pour A et B dans E, $(A \subset B) \leftrightarrow  (\complement_{B} \subset \complement_{A} )$ par double implication. Ajouter la démonstration détaillée ici ou dans [[MT02]].

### intersection
 #definition 
 Soient A et B deux ensembles, l'intersection est $A \cap B$
$$
(A \cap B) \leftrightarrow (x \in A \wedge x \in B)
$$
### union
Soient A et B deux ensembles, l'intersection est $A \cup B$
$$
(A \cup B) \leftrightarrow (x \in A \vee x \in B)
$$
### singleton
Un ensemble avec qu'un seul élément
exemple :
$$
R^+\cap R^-=\{ 0 \}
$$

### Exemples généraux
$$
R^+\cup R^-=R
$$
$$
(A \subset B) \implies (A \cap B = A)
$$

### Loi de Morgan
Soient A et B deux sous-ensemble de R, alors
$$
\complement_{A \cap B} = \complement_{A} \cup \complement_{B}
$$
$$
\complement_{A\cup B} = \complement_{A} \cap \complement_{B}
$$
#todo : Faire la démonstration des lois de Morgan en utilisant les propriétés logiques de la conjonction et disjonction. Ajouter la preuve détaillée ici ou dans [[MT02]].
$$
\neg(x \in A \cap B) \leftrightarrow  x \notin (A \cap B) \leftrightarrow (x \notin A) \vee (x \notin B)
$$

#propriété
soit A, B et C des ensembles
$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
#todo : Faire la démonstration de la distributivité de l'intersection sur l'union. Ajouter la preuve ici ou dans [[MT02]].

### La fonction caractéristique / indicatrice
#definition
Soit A un sous ensemble de E
On appelle fonction indicatrice de A relativement à E,
la fonction noté $\xi A(x) = 1$ si $x \in A$ 
et $\xi A(x) = 0$ si $x \not\in A$

#propriété
$$
\forall x \in E, \xi E(x)=1
$$$$
\forall x \in E, \xi\varnothing(x)=0
$$
$$
\forall x \in E, \xi\complement_{A} = 1-\xi A(x)
$$
$$
(A = B) \leftrightarrow (\xi A = \xi B)
$$ il faut montrer que $\forall x \in E, \xi A(x) = \xi B(x)$
#todo : Revoir le reste des propositions dans [[MT02-ch1_ecran.pdf]]. Faire l'application avec $(A \cap B) \cap C = A\cap(B\cap C)$ et montrer que $\xi_{A\cap B \cap C} = \xi_{A} \cdot \xi_{B} \cdot \xi_{C}$ en utilisant les propriétés de l'indicatrice.