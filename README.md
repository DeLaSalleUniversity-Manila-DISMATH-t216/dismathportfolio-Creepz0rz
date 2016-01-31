# My Dismath Portfolio
dismathportfolio-Creepz0rz created by Classroom for GitHub

## Week 1
* Discrete mathematics (DISMATH) is a subject, used to arrive at a mathematical truth of a statement
* DISMATH uses logic symbols shown in this table:

| Logical Symbol  |  Logical Operator | Shorthand | Logical Expression |
| :-----: |:-------:|:-----:| :-------: |
| ¬ | Negation | NOT | ¬p |
| ∧ | Conjunction | AND | p ∧ q |
| v | Disjunction | OR | p v q |
| ⊕ | Exclusive disjunction | XOR| p ⊕ q  ≡ (¬p ∧ q) v (p ∧ ¬q) |
| → | Conditional | IF, THEN | p → q ≡  ¬p v q |
| ↔ | Biconditional | IFF |  p ↔ q ≡ (p → q) ∧ (q → p) |

Notes:
* Conditional
  * q is always true, or p must be also false
* Biconditional
  * p and q must be opposite


## Week 2
###Logical Equivalences

 * used for more complex logical statements for proving

| Name  | Logical Equivalence |
| :-----: | :-------: |
| Identity | p v F ≡ p
|   |  p ∧ T ≡ p  |
| Domination  | p v T ≡ T |
|   | p ∧ F ≡ F | 
| Negation | p v ¬p ≡ T |
|  | p ∧ ¬p ≡ F |
| Double Negation | ¬(¬p) ≡ p |
| Idempotent | p v p ≡ p |
|  | p ∧ p ≡ p |
| Commutative | p v q ≡ q v p |
|  | p ∧ q ≡ q ∧ p |
| Associative | (p v q) v r ≡ p v (q v r) |
|  | (p ∧ q) ∧ r ≡ p ∧ (q ∧ r) |
| Distributive | p v (q ∧ r) ≡ (p v q) ∧ (p v r) |
|  | p ∧ (q v r) ≡ (p ∧ q) v (p ∧ r) |
| De Morgan's | ¬(p ∧ q) ≡ ¬p v ¬q |
|  | ¬(p v q) ≡ ¬p ∧ ¬q |
| Absorption | p v (p ∧ q) ≡ p |
|  | p ∧ (p v q) ≡ p |

Notes:
*Laws are reversible
* From identity/domination law, it is assumed that

>  F < p < T

Because:
 * v is for the maximum value
 * ∧ for the minumum 


Other "laws"

| Name  | Logical Equivalence |
| :-----: | :-------: |
| Implication Equivalence | p → q ≡ ¬p v q|
| Using Negation on T and F | ¬T ≡ F |
|   | ¬F ≡ T | 

### Quantifiers 

|Name| Statement | Condition |
| :-----: | :-------: | :-------: |
|Universal Quantifier| ∀x.p(x) | x is true for all values|
|Existential Quantifier| ∃x.p(x) | x is true for a certain value/s |

### Rules of Inference


## Week 3

### Methods of Proof
* Direct Proof
* Proof by Contraposition (Indirect)
* Vacuous and Trivial Proof
* Proof by Contradiction (Indirect)
* Proof by Equivalence
* Mathematical Induction
