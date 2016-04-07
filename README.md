# My Dismath Portfolio
dismathportfolio-Creepz0rz created by Classroom for GitHub  
Written by: Jason M. Tan

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
* Exclusive disjunction
 * p and q must be opposite
* Conditional
  * q is always true, or p must be also false
* Biconditional
  * q and p must both be true/false


## Week 2
###Logical Equivalences

 * used for more complex logical statements for proving

| Law  | Logical Equivalence |
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
| Contrapositive | p → q ≡ ¬q → ¬p|

### Quantifiers 

|Name| Statement | Condition |
| :-----: | :-------: | :-------: |
|Universal Quantifier| ∀x.p(x) | x is true for all values|
|Existential Quantifier| ∃x.p(x) | x is true for a certain value/s |

### Rules of Inference

| Name  | Rule | Tautology|
| :-----: | :------- | :--------: |
| Modus Ponens | p | (p ∧ (p → q)) → q |
| |  p → q  | |
| | ∴ q | |
| Modus Tollens |¬q | (¬q ∧ (p → q)) → ¬p |
| | p → q| |
| | ∴ ¬p | |
|Hypothetical Syllogism | p → q| ((p → q) ∧ (q → r)) → (p → r) |
| | q → r | |
| | ∴ p → r | |
| Disjunctive Syllogism | p ∨ q | ((p ∨ q) ∧ ¬p) → q |
| | ¬p | |
| |∴ q | |
| Addition | p | p → p ∨ q |
| | ∴ p ∨ q |
| Subtraction | p ∧ q | (p ∧ q) → p |
| | ∴ p |
| Conjunction | p | ((p) ∧ (q)) → (p ∧ q) |
| | q |
| | ∴ p ∧ q |
| Resolution | p ∨ q | ((p ∨ q) ∧ (¬p ∨ r)) → q ∨ r |
| | ¬p ∨ r |
| | ∴ q ∨ r |

## Week 3

### Methods of Proof
* Direct Proof
* Proof by Contraposition (Indirect)
* Vacuous and Trivial Proof
* Proof by Contradiction (Indirect)
* Proof by Equivalence
* Mathematical Induction

#### Direct Proof
Steps:

1. Assume p = T
2. Following the statement:   

>  p → q   

Prove that q = T so (p → q) = T

#### Proof by Contraposition
Steps:

1. Assume ¬q = T
2. Following the statement:   

>  ¬q → ¬p (from the contrapositive rule)    

Prove that ¬p = T so (¬q → ¬p) = T
## Week 3

#### Vacuous Proof

Following the statement:   

>  ¬p → (p → q)

Prove that p = F so ¬p → (p → q) = T

#### Trivial Proof

Following the statement:   

>  q → (p → q)

Prove that q = T so q → (p → q) = T

#### Proof by Contradiction
 * Not the same as Contraposition

1. Assume ¬p = T     
2. Make a contradiction from the previous assumption, proving that p = T and ¬p = F

* p may be a whole premise or statement

## Week 4

#### Proof by Equivalence

>  p ↔ q

1. Based on the Biconditional statement, we must also prove that:

>  p → q = T & q → p = T for {(p ↔ q) ↔ [(p → q) ∧ (q → p)]} = T


#### Bonus: Counterexample
 * Use any value to disprove the equation entirely
 
 
#### Mathematical induction

1. Basis Step: prove that P(1) = T
2. Inductive step: assume that P(k) = T
3.  Prove that P(k+1) = T so P(n) = T
    *tip: use the assumption P(k) = T to substitute some of the values in P(k+1) to prove

END OF METHODS OF PROOF

## Week 5

#### Recursive definition  

1. Basis Step: Specify the value of the function at zero.  
2. Recursive Step: Give a rule for finding its value at an integer from its values at smaller integers.  

  Simply put: Substitute values to get the next number  

#### Program Correctness

Goals:  
1. To get the correct output q from input p  
2. Program needs to terminate  

 Use the Hoare triple {p}C{q} to verify correctness   
  - substitute p with the input, C for the command/s, q for the output   

#### Sets

 1. A collection of objects
   - Objects may be other sets too (and counted as such too)   
   - Copies of the same object is counted as one single object   
   - Sets with no objects inside are called null sets   

 2. Power sets   
   - Basically a set with all of the possible subsets from a single set specified  

 3. Set operations  
   - Almost the same as logical equivalences

 4. Set Cardinality  
   - The number of objects in a set  
   - If it is infinite, it is ℵ₀ (aleph-nought)  
   - If two sets can have all of its objects paired together, it means they have the same cardinality   


## Week 6  
#### Functions  

Definition:  

 with two sets A & B, function f(A)=B means that A's objects will be assigned to objects to set B.  
  - Note: A can only assign one object, but B can have multiple objects assigned to one of the set's objects  


Other terms:   

Domain - The input function (In f(A)=B, A is the domain)  
Codomain - The output function (In f(A)=B, b is the codomain)  
Image - the resulting element from the element it was assigned to  
Range - The list of objects from the resulting set that was only assigned to from the domain   

Types:  

1. One-to-one Function (Injective)  
 - Functions that only assign strictly one object/element to the codomain  

2. Onto Function (Surjective)  
 - The range is equal to the codomain (all elements from the codomain is used, regardless of how many objects from the domain it was assigned  

3.One-to-one Correspondence (Bijection)  
 - If a function is both one-to-one and onto, it is One-to-one Correspondence

## Week 8  

#### Algorithms  

#####Search Algorithms    

Linear Search    

 - Searches variables one-by-one until it find the value exact to what it was searching for, else value will not be found. No need to sort variable list  

Binary Search    

 - Searches variables by finding the midpoint, and checking if the searching variable is above/below the midpoint, then halves the list to the supposed contained variable. this is repeated until there is only one variable left and cannot be halved. If searched variable is the same, it will be the variable found, else it is not found. Note: Use binary search only on sorted lists  
  
## Week 9   
 
#####Sorting Algorithms     
 
Bubble Sort   
  
 - Compare two values, switch values if it is greater, else leave as is. continue to step up by +1, until it reaches the end. Last number that reaches the end will "lock", to prevent redundant comparisons. For succeeding loops, compared numbers at the edge will lock if it is beside a locked number. This will continue until all numbers are locked in place  
 
 - "the biggest bubble will rise to the top"  

Insert Sort   

 - Compare a value to all values, it will "insert" itself if the value is greater than the value the algorithm was holding. repeat until all values are sorted.  

Greedy sort    

 - Search for the highest number first for it to be placed in the end, then searches the next highest number to put it beside the actual highest number. repeat until all values are sorted
 
## Week 10  
#### Growth Of Functions  
Big O: checks if it can go above the supposed function at any time  (higher bound)  
Big Omega: if it can go below the supposed function at any time  (lower bound)  
Big Theta: checks if it can both above and below the supposed function at any time  (higher and lower bound)  
    
Proof: Show witnesses c and K  

  
## Week 12  
#### Graph Theory   

Two parts: Nodes (vertices) and edges (lines)    

Notation:  G = (V,E), V=(V1,12,...Vn), E=(E1,E2,... En)  

Terminology:    
Endpoints - points the edge contains   
Adjacent - two vertices with the same node   
Incident - edge is connected to either endpoint of another edge   

Degree - The number of edges in a vertex   
  0 Degree Vertex- Isolated  
  1 Degree Vertex - Pendant  

Handshaking Theorem  
> E = (VxD)/2   
 E = Edges    
 V = Vertices  
 D = Degree  
 
Special Graphs:  
 n = number of vertices  
 
Kn - One edge between each distinct endpoints   
Cycle (Cn) - Edges are only connected to vertices next to each other ({V1,V2}, {V3,V4}, {V5,V6},.... {Vn-1, Vn} until {Vn, V1})   
Wheel (Wn) - In addition to Cycle, but has a center vertex which all vertices are connected to it   
Star (Sn) - there is one central vertex, and all other vertices are connected to it, but other vertices aren't connected to each other ({V1,V2}, {V1,V2}, {V1,V3}, {V1, Vn})   

Union - combination of two graphs    

Path - A sequence of nodes that pass through the edges  

Euler Circuits  
 - A path that contains every edge in Graph G, but also terminates at the point started to induce a loop.    
 - It is only an Euler path if the path does not terminate at the start of the path      
   
Heuristics(Euler Circuits):   
Euler circuit will only have vertices of even degree else--  
Euler path will only have two vertices of odd degree  

Hamilton Circuits  
- Same as euler circuits, but checks nodes instead of edges  
- Same applies for Hamilton Paths  
  
  Note: It does not need to pass all edges for it to become a Hamilton circuit/path    

Heuristics (Hamilton Circuits):    
- No pendants for circuits, but about two maximum for paths  
  
## Week 13

#### Graph Theory(Continued)   

Matrices of Graphs   
 - Just plot a matrix with size of number of variables(vertices), then check each connection for each vertice comparing to another, 1 if connected else 0  

Isopmorphism  
- Comparing two graphs to have the same number of nodes and edges, and same degree on each node      

Planar Graphs - Graph that has no edges that intersect (not inbetween nodes)    

Euler's formula:  r = e-v-2    
 r - Regions (faces) of the graph  
 e - edges   
 v - vertices   

Homeomorphic Graphs  
 - "turn" edges into separate vertices and edges  

Kuratowski's Theorem  
 - A graph is nonplanar if a subgraph is also nonplanar
 
Graph Coloring   
 - Placing a color on each vertice, but no two colors can be adjacent to each vertice    
 - Chromatic number: the amount of colors a graph has    
  
Trees    
 - a graph with no circuits  
 - M-ary tree - vertices in trees have no more than m children  
 
