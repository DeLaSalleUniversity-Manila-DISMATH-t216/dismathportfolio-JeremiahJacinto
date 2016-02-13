# dismathportfolio-JeremiahJacinto
dismathportfolio-JeremiahJacinto created by Classroom for GitHub

##Week1
- A proposition is a statement that is either true (1) or false (0).
- An axiom is a statement or proposition that is regarded as being established, accepted, or self-evidently true.

| Logical Symbol  |  Logical Operator     | Shorthand | Formula                                       | Logical Expression             |
| :-------------: |:---------------------:|:---------:|:---------------------------------------------:|:-----------------------------:|
| ¬               | Negation              | not       | val(¬p) = 1 - val(p)                          | ¬p                           |
| ∧               | Conjunction           | and       | val(p ∧ q) = min(val(p), val(q))              | p ∧ q                          
| v               | Disjunction           | or        | val(p v q) = max(val(p), val(q))              | p v q                        |
| ⊕              | Exclusive disjunction | xor       | if val(p)  not equal val(q) = 1 , otherwise  0|  p ⊕ q  ≡ (¬p ∧ q) v (p ∧ ¬q) |
| →               | Conditional           | if, then  | if val(p)  ≤ val(q) = 1 , otherwise  0        | p → q ≡  ¬p v q              |
| ↔               | Biconditional         | iff       | if val(p) equals val(q) = 1 , otherwise  0    |  p ↔ q ≡ (p → q) ∧ (q → p)    |

- Disjunction gets the Maximum 
- Conjuction gets tha minimum
- In getting truth table = 2^n Where n is the number of propositional variables

NOTE:
- Logic diagrams not included in exam
- Bitwise Operation included in exam


##Week2

- Argument - a sequence of statements that end with a conclusion.
- Valid - the conclusion, or final statement of the argument, must follow from the truth of the preceding statements, or premises, of the argument.
- Fallacy - common form of incorrect reasoning which lead to invalid arguments.
- Existential quantifier (∃x) - "there exist"
- Universal quantifier - (∀x) - "for all"

|                           Equivalence                           |         Name        |
|:-------------------------------------------------------------:  |:-------------------:|
|                      p ∧ T ≡ p <br> p v F ≡ p                   |    Identity laws    |
|                       p v T ≡ T <br> p ∧ F ≡ F                  |   Domination laws   |
|                       p v p ≡ p <br> p ∧ p ≡ p                  |   Idempotent laws   |
|                            ¬(¬p) ≡ p                            | Double negation law |
|                   p v q ≡ q v p <br> p ∧ q ≡ q ∧ p              |   Commutative laws  |
|       (p v q) v r ≡ p v (q v r) <br> (p ∧ q) ∧ r ≡ p ∧ (q ∧ r)  |   Associative laws  |
| p v (q ∧ r) ≡ (p v q) ∧ (p v r) <br>  p ∧(q v r) ≡ (p ∧ q) v (p ∧ r) |  Distributive laws  |
|              ¬(p ∧ q) ≡ ¬p v ¬q <br> ¬(p v q) ≡ ¬p ∧ ¬q          |   De Morgan's laws  |
|                 p v (p ∧ q) ≡ p <br> p ∧ (p v q) ≡ p             |   Absorption laws   |
|                     p v ¬p ≡ T <br> p ∧ ¬p ≡ F                   |    Negation laws    |

MEMORIZE 
- p → q ≡  ¬p v q
- p ↔ q ≡ (p → q) ∧ (q → p)

NOTE:
 - ALWAYS CHECK THE ORDER OF PARENTHESIS
 
##Week3

|   Rule of Inference       |            Tautology           |          Name          |
|:--------------------:     |:------------------------------:|:----------------------:|
|       p<br>p→q<br>∴q      |        (p ∧ (p → q)) → q       |      Modus ponens      |
|     ¬q<br>p→q<br>∴ ¬p     |       (¬q ∧ (p → q)) → ¬p      |      Modus tollens     |
|     p→q<br>q→r<br>∴p→r    |  ((p → q) ∧ (q → r)) → (p → r) | Hypothetical syllogism |
|      p∨q<br>¬p<br>∴q      |       ((p ∨ q) ∧ ¬p) → q       |  Disjunctive syllogism |
|       p<br>∴p ∨ q         |           p → (p ∨ q)          |        Addition        |
|       p ∧ q<br>∴p         |           (p ∧ q) → p          |      Simplication      |
|      p<br>q<br>∴p ∧ q     |      ((p) ∧ (q)) → (p ∧ q)     |       Conjunction      |
| p ∨ q<br>¬p ∨ r<br>∴q ∨ r | ((p ∨ q) ∧ (¬p ∨ r)) → (q ∨ r) |       Resolution       |


##Week 4

Methods of Proof
1. Direct proof (p → q)
    - Assume p is T.
    - Show that q is also T.
2. Proof by contraposition (¬q → ¬p)
	 - Assume ¬q is T.
	 - Show that ¬p is also T.
3. Vacuous Proof (¬p → (p → q))
	 - Show that p is F
	 - p → q must be T.
4. Trivial Proof (q → (p → q))
	 - Show that q is T
	 - p → q is also T
	 
NOTE:
- Use Direct proof is p is more simple
- Use Contrapositive if p is complex


- Even number n = 2k
- Odd number n = 2k+1 / 2k -1

##Week5
5. Proof by contradiction
	 - Asuume that the premise is not T (¬premise ≡ T)
	 - Based on that, show that the premise will end up in a contradiction.   
6. Proof by Equivalence (p ↔ q = (p → q) ∧ (q → p)

NOTE:
- Proof by Contradiction : Apply Truth table in taking the negation of the premise.

##Week6
- You can disprove a theorem using counterexample.

Mathematical Induction
	    1. Basic step: Show P(1) ≡ T
	    2. Inductive step: 
	      - Assume P(k) is true.
	      - Show that is also P(k+1) true.

Prove P(n) = 1 + 2 + 3 + … + n = n(n+1)/2
	    - 1. Prove P(1) is true
	    - 2. Direct proof
	      - a. Assume P(k) ≡ T
	        - P(k) = 1 + 2 + 3 + … + k = k(k+1)/2
 	      - b. Show P(k + 1)
         - P(k + 1) = 1 + 2 + 3 + … + k + (k + 1) = (k+1)(k+2)/2
         
         Guide: P(k) = 1 + 2 + 3 + … + k = k(k+1)/2
         Substitute
	        - P(k + 1) = k(k+1)/2 + k + 1 =  (k+1)(k+2)/2
	        - P(k + 1) = (k+1)(k + 2)/2 =  (k+1)(k+2)/2
NOTE:
- Manipulate only 1 side.
