# Étude de Marché et Probabilité

**Énoncé :**

Une entreprise de télécommunications sait que 30% des clients contactés par téléphone acceptent de changer de fournisseur. L'entreprise décide de contacter 15 clients potentiels.

1. **Calcul de l'Espérance :**
   - Quel est le nombre moyen de clients qui acceptent de changer de fournisseur ?

2. **Calcul de Probabilité :**
   - Quelle est la probabilité que 6 clients exactement changent de fournisseur ?
  
3. **Calcul de Probabilité :**
   - Quelle est la probabilité que plus de 6 clients acceptent de changer de fournisseur, donnez la formule seulement.

**Correction :**

#### 1. Calcul de l'Espérance

- **Paramètres :**
  - $n = 15$ (nombre de clients contactés)
  - $p = 0.3$ (probabilité qu'un client accepte de changer de fournisseur)

- **Calcul de l'espérance :**
  $E(X) = np = 15 \times 0.3 = 4.5$

Le nombre moyen de clients qui acceptent de changer de fournisseur est de 4.5.

#### 2. Calcul de Probabilité

- **Probabilité que plus de 6 clients acceptent :**
  $P(X > 6) = P(X = 7) + P(X = 8) + \ldots + P(X = 15)$

- **Utilisation de la loi binomiale :**
  - Calculer $P(X = k)$ pour $k$ allant de 7 à 15.

- **Calcul détaillé :**
  - Utilisation de la fonction de masse de probabilité binomiale pour chaque $k$ de 7 à 15.

- **Calcul de la probabilité totale :**
  $P(X > 6) = \sum_{k=7}^{15} \binom{15}{k} \times 0.3^k \times (1-0.3)^{15-k}$

```python
from scipy.stats import binom

# Paramètres
n = 15
p = 0.3
k = 6

# Calcul de P(X > 6)
probabilite_x_sup_6 = binom.sf(k, n, p)

probabilite_x_sup_6
```