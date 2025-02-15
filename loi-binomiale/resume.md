# Loi Binomiale 

La loi binomiale est un concept fondamental en statistiques et en probabilités.

### Qu'est-ce que la loi binomiale ?

>[!IMPORTANT]
La loi binomiale est **une distribution de probabilité discrète** qui décrit le nombre de succès dans une séquence de $n$ essais indépendants, où chaque essai a deux issues possibles : succès ou échec.

### Paramètres de la loi binomiale

1. **$n$** : Le nombre d'essais ou d'expériences.
2. **$p$** : La probabilité de succès pour chaque essai.

### Conditions d'application

Pour qu'une situation soit modélisée par une loi binomiale, il faut que :
- Chaque essai n'ait que deux issues possibles : succès ou échec.
- La probabilité de succès $p$ soit la même pour chaque essai.
- Les essais soient indépendants les uns des autres.

### Formule de la loi binomiale

La probabilité d'obtenir exactement $k$ succès dans $n$ essais est donnée par la formule :

$P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$

où :
- $\binom{n}{k}$ est le coefficient binomial, qui se lit "n choisit k" et se calcule comme $\frac{n!}{k!(n-k)!}$.
- $p$ est la probabilité de succès.
- $(1-p)$ est la probabilité d'échec.

### Espérance et variance

- **Espérance** : $E(X) = np$
- **Variance** : $\text{Var}(X) = np(1-p)$

### Exemple d'application

Imaginons que vous lancez une pièce de monnaie équilibrée 10 fois ($n = 10$) et que vous souhaitez calculer la probabilité d'obtenir exactement 6 fois face ($k = 6$). La probabilité de succès (obtenir face) est $p = 0.5$.

La probabilité d'obtenir exactement 6 faces est :

$P(X = 6) = \binom{10}{6} (0.5)^6 (0.5)^{4}$

Remarque: si vous avez 4 lancers et que l'on souhaite calculer le nombre de fois que l'on obtient 2 fois faces, on a alors les combinaisons possibles suivantes: 

FFPP est une possibilité de lancer, mais FPFP en est une autre. Si on cherche à les énumérer toutes, ici, on peut encore le faire facilement.

$\binom{4}{2} = \frac{4!}{2!(4-2)!}=\frac{4*3*2*1}{2*1(2*1)!}=6$

En les comptant à la main :

- FFPP
- PFFP
- PPFF
- FPFP
- PFPF
- FPPF

## Application

La loi binomiale peut être utilisée pour modéliser des situations de gestion ou de marketing, comme :
- La probabilité qu'un certain nombre de clients achètent un produit lors d'une campagne publicitaire.
- Le nombre de défauts dans un lot de produits fabriqués.
