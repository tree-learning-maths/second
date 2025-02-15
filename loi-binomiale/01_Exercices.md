# Exercices

### Exercice 1 : Lancer de Dé

**Énoncé :**

Un dé équilibré à 6 faces est lancé 4 fois. Quelle est la probabilité d'obtenir exactement 2 fois le chiffre 6 ?

**Correction :**

1. **Identification des paramètres :**
   - Nombre d'essais $n = 4$
   - Nombre de succès $k = 2$
   - Probabilité de succès $p = \frac{1}{6}$ (puisque le dé est équilibré)

2. **Calcul du coefficient binomial :**
   $\binom{4}{2} = \frac{4!}{2!(4-2)!} = \frac{4 \times 3}{2 \times 1} = 6$

3. **Calcul de la probabilité :**
   $P(X = 2) = \binom{4}{2} \left(\frac{1}{6}\right)^2 \left(\frac{5}{6}\right)^2 = 6 \times \frac{1}{36} \times \frac{25}{36} = \frac{150}{1296} = \frac{25}{216}$

La probabilité d'obtenir exactement 2 fois le chiffre 6 en lançant un dé 4 fois est donc $\frac{25}{216}$, soit environ $0.116$ ou $11.6\%$.

### Exercice 2 : Campagne Publicitaire

**Énoncé :**

Une entreprise sait que 30% des clients contactés par téléphone achètent un produit. Elle appelle 8 clients. Quelle est la probabilité que 5 clients exactement achètent le produit. Puis calculez la probabilité que 5 clients ou plus achètent le produit ?

**Correction :**

1. **Identification des paramètres :**
   - Nombre d'essais $n = 8$
   - Probabilité de succès $p = 0.3$

2. **Calcul des probabilités pour $k = 5, 6, 7, 8$ :**

   - Pour $k = 5$ :
     $P(X = 5) = \binom{8}{5} (0.3)^5 (0.7)^3$

Réponse à la première question :  $P(X = 5) = \binom{8}{5} (0.3)^5 (0.7)^3$

Pour répondre à la deuxième question on calcule les autres probabilités. 

   - Pour $k = 6$ :
     $
P(X = 6) = \binom{8}{6} (0.3)^6 (0.7)^2
$

   - Pour $k = 7$ :
     $
P(X = 7) = \binom{8}{7} (0.3)^7 (0.7)^1
$

   - Pour $k = 8$ :
     $
P(X = 8) = \binom{8}{8} (0.3)^8 (0.7)^0
$

1. **Calcul de la probabilité totale :**
   $P(X \geq 5) = P(X = 5) + P(X = 6) + P(X = 7) + P(X = 8)$


La probabilité que 5 clients ou plus achètent le produit est donc d'environ $0.126$ ou $12.6\%$.

### Exercice 3 : Probabilité d'un Nombre Exact de Succès

**Énoncé :**
Un magasin sait que 40% des clients qui entrent achètent un produit spécifique. Si 10 clients entrent dans le magasin, quelle est la probabilité que 5 d'entre eux achètent le produit ?

**Correction :**

1. **Paramètres :**
   - $n = 10$ (nombre de clients)
   - $k = 5$ (nombre de succès)
   - $p = 0.4$ (probabilité d'achat)

2. **Calcul de la probabilité :**
   $P(X = 5) = \binom{10}{5} \times 0.4^5 \times (1-0.4)^{10-5}$

3. **Calcul détaillé :**
   - Coefficient binomial : $\binom{10}{5} = 252$
   - $p^5 = 0.4^5 = 0.01024$
   - $(1-0.4)^5 = 0.6^5 = 0.07776$
   - Probabilité totale : $P(X = 5) = 252 \times 0.01024 \times 0.07776 \approx 0.2007$

La probabilité que 5 clients sur 10 achètent le produit est environ $0.2007$ ou $20.07\%$.

### Exercice 4 : Probabilité d'un Nombre de Succès Supérieur à une Valeur

**Énoncé :**
Une entreprise sait que 30% de ses produits fabriqués sont défectueux. Si l'entreprise fabrique 8 produits, quelle est la probabilité que plus de 4 produits soient défectueux ?

**Correction :**

1. **Paramètres :**
   - $n = 8$ (nombre de produits)
   - $p = 0.3$ (probabilité de défectuosité)

2. **Calcul de la probabilité :**
   $P(X > 4) = P(X = 5) + P(X = 6) + P(X = 7) + P(X = 8)$

3. **Calcul détaillé :**
   - Utilisation de la fonction de masse de probabilité binomiale pour chaque $k$ de 5 à 8.
   - Probabilité totale : environ $0.0580$

La probabilité que plus de 4 produits sur 8 soient défectueux est environ $0.0580$ ou $5.80\%$.
