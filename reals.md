---
title: The real numbers
---

The set, $\mathbb{R}$, of real numbers is the set of numbers corresponding to points on the continous one-dimensional number line. They are a fundamental mathematical object and lie at the heart of calculus and it use in the modelling of the real world through physics and the other sciences. 

## Constructing the reals

One can approach the real numbers in different ways. They can be *constructed* using set-theoretic methods from the rational numbers $\mathbb{Q}$, the set of all quotients of integers, which in turn can be constructed from the integers, $\mathbb{Z}$, which in turn are constructed from the naturals or counting number $\mathbb{N}$. 

The two main methods of constructing the reals from the rationals are [Cauchy sequences](https://en.wikipedia.org/wiki/Cauchy_sequence) and [Dedekind cuts](https://en.wikipedia.org/wiki/Dedekind_cut). These constructions would be studied in course on Real Analysis. 

## Axioms for the reals

But one can also define, or characterize, the reals in an axiomatic way, as the unique *complete ordered field*. A complete ordered field is an algebraic structure consisting of a non-empty set
$F$, with two distinguished elements $0$ and $1$, and $F$ carries two binary operations of *addition*, $+$, and *multiplication*, $\cdot$, and a binary relation of *inequality*, $\leq$, all of which satisfy the following axioms.

### Axioms about $+$ and $\cdot$ on $F$.

1. Addition is *associative*, i.e. $$\forall \, x,y,z \in F \quad x+(y+z) = (x+y)+z.$$
2. Existence of an *additive identity*, i.e. $$ \exists \, 0 \in F \, \, \forall \, x \in F \quad x+0 = 0+x =x.$$
3. Existence of *additive inverses*, i.e. $$ \forall \, x \in F \, \, \exists \, -x \in F \quad x + (-x) =(-x)+x = 0.$$
4. Addition is *commutative*, i.e. $$ \forall \, x,y \in F \quad x+y = y+ x.$$
5. Multiplication is associative, i.e. $$\forall \, x,y,z \in F \quad x \cdot (y \cdot z) = (x \cdot y) \cdot z.$$
6. Existence of a *multiplicative identity*, i.e. $$ \exists \, 1 \in F \quad 1 \neq 0 \text{ and } \forall \, x \in F \quad 1 \cdot x = x \cdot 1 = x.$$
7. Existence of *multiplicative inverses*, i.e. $$ \forall \, x \in F \, \, x \neq 0 \Rightarrow \exists \, x^{-1} \in F \quad x \cdot x^{-1} =x^{-1} \cdot x = 1.$$
8. Multiplication is *commutative*, i.e. $$ \forall \, x,y \in F \quad x \cdot y = y \cdot x.$$
9. Multiplication *distributes* over addition, i.e. $$\forall \, x,y,z \in F \quad x \cdot(y+z) = (x \cdot y) + (x \cdot z).$$

### $F$ is totally ordered by $\leq$.

10. $\leq$ is *reflexive*, i.e. $$\forall \, x \in F \quad x \leq x.$$
11. $\leq$ is *anti-symmetric*, i.e. $$\forall \, x,y \in F \quad \big ( x \leq y \text{ and } y \leq x \big ) \Rightarrow x=y.$$
12. $\leq$ is *transitive*, i.e. $$ \forall \, x,y,z \in F \quad \big ( x \leq y \text{ and } y \leq z \big ) \Rightarrow x \leq z.$$
13. *Totality* of $\leq$, i.e. $$\forall \, x,y \in F \quad x \leq y \text{ or } y \leq x.$$

### Axioms about how $+$ and $\cdot$ are compatible with $\leq$

14. Addition *preserves* order, i.e. $$\forall \,  x,y,z \in F \quad x \leq y \Rightarrow x+z \leq y+z.$$ 
15. Multiplication *preserves* order, i.e. $$\forall \,  x,y  \in F \quad \big ( 0 \leq x \text{ and } 0 \leq y \big ) \Rightarrow 0 \leq x \cdot y.$$ 

### Completeness axiom or the least upper bound axiom

16. If $G$ is a non-empty subset of $F$ that is *bounded above*, then $G$ has a *least upper bound*.
    * $G$ is *bounded above* means $$\exists \, v \in F \, \, \forall \, g \in G \quad g \leq v.$$
    * $u$ is a *least upper bound* for $G$ means, if $v$ is an upper bound for $G$, then $u \leq v$.
