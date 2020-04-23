# Set Theory

Set theory is arguably the foundation of all mathematics. It is a mathematical discipline that deals with the logic of sets. Initiated by Georg Cantor in the 1870s when he made amazing discoveries that the linear continuum, the real line, is not countable, meaning that its points cannot be counted against natural numbers. 

Set theory is often used as a foundational system for mathematics, particularly in the form of Zermelo-Fraenkel set theory with the axiom of choice. Contemporary research into set theory includes a diverse collection of topics, ranging from the structure of the real number line to the study of the consistency of large cardinals.

## Basic Concepts

A set is a well-defined collection of objects called *elements*. Well-defined meaning that it is possible to know for certain if something belongs to the collection or not without prejudice.

There are a few ways to describe sets:
1. **verbal method**: use a sentence to describe a set
  - the set of all printed, 2nd edition magic the gathering cards
  - the set that contains all the letters that make up the word "concept"
2. **roster method**: list each element of the set only once then enclose all these with opening and closing braces
  - $\text{\{ c, e, n, o, p, t \}}$
  - $\{ \{ \text{Head, Tail} \},\ \text{Head},\ \text{Tail},\ \emptyset \}$

3. **set-builder method**: a combination of verbal and roster methods with a stand-in variable
  - $\{ x | x\ \text{is a letter in the word concept} \}$
  - $\{ x | x \geq 0 \}$

The set containing every possible object that we consider in a certain situation is called the universe and is usually denoted as $\Omega$. If an object $x$ is in $\Omega$ belongs to set $A$, we say that $x$ is an element of $A$ and write $x \in A$. If $x$ is not an element of $A$ then we write $x \notin A$.

The empty set, usually denoted by $\emptyset$, is a set such that $x \notin $ for all $x \in \Omega$.

If all elements in a set $B$ also belong to set $A$, then $B$ is a subset of $A$, which we denote by $B \subseteq A$. If in addition, there is at least one element in A that is not in $B$, then $B$ is a proper subset of $A$ and we write $B \subset A$. Two sets are equal if they have the same elements, $A = B$ if and only if $A \subseteq B$ and $B \subseteq A$. It is easy to verify for instance that $(A^c)^c = A, B \cup \Omega = \Omega, B \cap \Omega = B$.

The elements of a set can be arbitrary objects and in particular, they can be sets themselves. This is the case for the power set of a set. A useful way of defining a set is through statement concerning its elements. Let $A$ be the set of elements such that a certain statement $a(x)$ holds, to define $A$ we write: $A := \{x|a(x)\}$

For example, $A := \{ x | 1 < x < 3\}$ is the set of all elements greater than 1 and smaller than 3.

If $A$ is a finite set, we write |$A$| to denote the number of elements in $A$.

### Definition: Set Union

> The union of two sets $A$ and $B$ contains the objects that belong to $A$ or $B$
>
> $ A \cup B := \{ x | x \in A\ or\ x \in B \} $
>
> This can be generalized to a sequence of sets $A_1, A_2, ...$
>
> $ \bigcup_i^{\infty} A_i := \{ x | x \in A_i\ for\ at\ least\ one\ i \} $
>
> where the sequence may be infinite

#### Definition: Set Intersection

> The intersection of two sets $A$ and $B$ contains the objects that belong to $A$ and $B$
>
> $ A \cap B := \{ x | x \in A\ and\ x \in B \} $
>
> This can be generalized to a sequence of sets $A_1, A_2, ...$
>
> $ \bigcap_n A_n := \{ x | x \in A_n\ for\ all\ n \}  $
>
> where the sequence may be infinite. Sometimes we write $A \cap B$ as $AB$ or $(A,B)$

We say that $A$ and $B$ are disjoint or are mutually exclusive if $A \cap B = \emptyset$. For example $A = (0, 1]$ and $B = [-1, 0)$ are disjoint.

### Definition: Set Difference

> The difference of two sets $A$ and $B$ contains the elements in $A$ that are not in $B$
>
> $ A \setminus B := \{ x | x \in A\ and\ x \notin B \} $

### Definition: Power Set $2^A$

> The power set $2^A$ of a set $A$ is the set of all possible subsets of A, including $\emptyset$ and $A$.
> $ 2^A := \{ A' | A' \subseteq S\} $

### Definition: Cartesian Product

> The cartesian product of two sets $A$ and $B$ is the set of all ordered pairs of elements in the sets
>
> $ A \times B := \{ (x_1, x_2) | x_1 \in A, x_2 \in B \} $

As an example, $\mathbb{R}^2 = \mathbb{R} \times \mathbb{R}$, the set of all possible pairs of real numbers.

### Definition: Set Partition

> A partition of $\Omega$ is a sequence of disjoint sets $A_1, A_2, ...$ such that $\cup_{i=1}^{\infty} A_i = \Omega$

### Definition: Indicator Function

> Given an event $A$, an indicator function of $A$ is defined as
>
> $ I_A(\omega) = I(\omega \in A) = \begin{cases}
1\ if\ \omega \in A
\\ 0\ if\ \omega \notin A
\end{cases}
$

### Theorem: De Morgan's Laws

> For any two sets $A$ and $B$
>
> $\begin{align}
(A \cup B)^c &= A^c \cap B^c, 
\\ (A \cap B)^c &= A^c \cup B^c, 
\end{align}$

Proof. First we prove that $ (A \cup B)^c = A^c \cap B^c $. A standard way to prove the inclusion of a set in another is to show that if an element belongs to the first set then it must also belong to the second set. If the set is empty then the inclusion holds trivially, since $\emptyset \subseteq S$ for any set S. Any element $x \in (A \cup b)^c$ is in $A^c$ otherwise it would belong to $A$ and consequently $A \cup B$. Similarly, $x$ also belongs to $B^c$. We conclude that $x$ belongs to $A^c \cap B^c$, which proves the inclusion.

To complete the proof, we establish $A^c \cap B^c \subseteq (A \cup B)^c$. If $x \in A^c \cap B^c$, then $x \notin A$ and $x \notin B$, so $x \notin A \cup B$ and consequently $x \in (A \cup B)^c$.

## Borel Set

A Borel set is any set in a topological space that can be formed from open sets through the operations of countable union, countable intersection and relative complement. It was named after Emile Borel.

For a topological space $X$, the collection of all Borel sets on $X$ forms a $\sigma$-algebra, known as the Borel algebra. The Borel algebra on $X$ is the smallest $\sigma$-algebra containing all open sets (or equivalently, all closed sets).

Borel sets are important in measure theory since any measure defined on the open sets of a space (or on the closed sets of a space) must also be defined on all Borel sets of that space. Any measure defined on the Borel sets is called a Borel measure. Borel sets and the associated Borel Hierarchy also play a fundamental role in descriptive set theory.

> For a collection $T$ of subsets of $X$ (that is for any subset of the power set P(X) of X) let:
> - $T_{\sigma}$ be all countable unions of elements of $T$
- $T_{\delta}$ be all countable intersections of elements of $T$
- $T_{\delta\sigma} = (T_{\delta})_{\sigma}$
>
> Now define by transfinite induction a sequence $G^m$, where $m$ is an ordinal number, in the following manner:
> - For the base case of the definition, let $G^0$ be the collection of open subsets fo $X$.
- If $i$ is not a limit ordinal, then $i$ has an immediately preceding ordinal $i-1$: $\begin{align} G^i = [G^{i-1}]_{\delta\sigma} \end{align}$
- If $i$ is a limit ordinal set:
$\begin{align} G^i = \bigcup_{j < i}G^j \end{align}$

The claim is that the Borel algebra $G^{\omega}$, where $\omega_1$ is the first uncountable ordinal number. That is, the Borel algebra can be generated from the class of open sets by iterating the operation $G \mapsto G_{\delta\sigma}$ to the first uncountable ordinal.