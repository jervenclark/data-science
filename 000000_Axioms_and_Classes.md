# Axioms and Classes

## Classes, Sets and Axioms

### Statements

In Mathematics, a statement is a declaration that can be assigned a truth value. Meaning, a statement is either true or false. It cannot be both. There is a set of rigorous logical rules used to determine the truth value of each statement. 

Arguments that does not respect these rules are illogical. We can also combine these different rules to get the truth values of other mathematical statements. They often occur in this form:

> If $Q$ is true whenever $P$ is true, and $T$ is true whenever $Q$ is true, then $T$ is true whenever $P$ is true.

Rules like these are symbolically represented in a way that words are avoided to prevent ambiguity and unnecessary confusion:

> $$ [(P \implies Q) \land (Q \implies T)] \implies T $$

The logical steps used to determine the whether a statement is true or false are called proofs. If the truth value of a statement can be logically deduced by combining multiple statements previously known to be true, then at some point, there must be a set of statements whose truth values not previously derived from previous statements. That is, the process must start somewhere and there must be some initial statements declared to be true rather than derived.

For example, one may declare the statement "There is a set such that no element is a member of it." as being self-evident or too atomic that it cannot be proved. A statement like this is called an axiom. Once we give ourselves $\mathscr{A}$ of self-evident statements, then the universe $\mathscr{U}_{\mathscr{A}}$ of all possible true statements derived from $\mathscr{A}$ is determined. This determined universe of statements constitutes a mathematical theory which is ours to explore and discover.

But, suppose the choice of our original set $\mathscr{A}$ of statements was not wise? For example, say that a set $\mathscr{A}$ of initial self-evident statements, a statement $A$ has been shown to be true, and given $A$ we can deduce the statement $B$ to be also true and from $B$, $C$ must also be true. On the other hand it is shown that from $A$ we can show that $D$ is true but from $D$ we can deduce that $C$ is false. Hence, from $A$ we have deduced the values of $P$ to be both true and false.

This statement which has been determined to be both true and false is referred to as a contradiction or a paradox. If a contradictory statement logically flows from what was assumed to be a paradox-free system, then the initial statements used as the foundation of the mathematical system must be scrutinized to determine the incorrect assumptions.

### Sets

A set is a collection of objects called *elements* often described in terms of certain properties shared by each elements. These properties muse be well-defined , with no ambiguities, so that it is possible to know for certain if something belongs to the collection or not without prejudice. Being a *set* can also be an element property so sets whose elements are sets exists.

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

The way sets are defined along with their universally accepted properties from the foundation of modern mathematics. 

As mentioned earlier, a paradox consists of two contradictory statements both of which logically flow from what was thought to be a well understood and clearly defined concept. For example, the statement $S$ is an element of $S$ is true means that the statement $S$ is and element of $S$ is false, and vice-versa. For many, this would mean nothing more than a play on words and may seem harmless enough. For mathematicians, however, it is not a trivial matter that cannot be ignored.

Paradoxes such as this undermines the confidence we have in mathematics, a discipline which prides itself on its clarity. Once this flaw was exposed it is important to understand why we did not see this before and whether there are any other cracks requiring immediate attention.

But the crux is, how do we decide which assumptions are acceptable and which ones are not? This problem motivated mathematicians to determine as clearly as possible what are acceptable properties of sets. Since most of modern mathematics can be derived from the notion of sets, this question was labeled as a high priority in the early 1900s. It is in this period that particular attention was given to develop a reliable axiomatic system.

### Axiomatic Systems

An axiomatic system is normally set up by first declaring atomic statements or primitive concepts. These primitive concepts carry no intrinsic meaning although the symbols or words used to represent them often convey some intuitive concept in the mind of the reader. Meaning that the words representing this undefined notion are such that the user will easily understand the properties which will be prescribed for this concept.

Specific rules and properties which declare how these concepts relate to each other are then formulated; these rules and properties must allow mathematical constructs which are viewed as being important in our mathematical system. These are called axioms.

### Euclid's Axiomatic System

Euclid provided us with a useful model for constructing an axiomatic system. He is the first person to apply the axiomatic method of defining a certain field of study. In his axiomatic system, the words *line* and *point* are primitive concepts. These properties are his axioms. 

An interesting question about Euclid's system of geometry is the difference between an axiom and a postulate. *Axioms* from Greek axíôma, "worthy" is in some sense thought to be strongly self evident while a *postulate* on the other hand is simply postulated. For a postulate, there need not be a notion of truth, just the declaration that we are going to do it this way and see what happens.

Euclid's postulates, indeed, could be thought of as those assumptions that were necessary and sufficient to derive truths of geometry, of some of which we might otherwise already be intuitively persuaded. As first principles of geometry, however, both axioms and postulates, on Aristotle's understanding, would have to be self-evident. This never seemed entirely quite right, at least for the Fifth Postulate -- hence many centuries of trying to derive it as a Theorem. 

*Euclid's Axioms*

- First Axiom: Things which are equal to the same thing are also equal to one another.
- Second Axiom: If equals are added to equals, the whole are equal.
- Third Axiom: If equals be subtracted from equals, the remainders are equal.
- Fourth Axiom: Things which coincide with one another are equal to one another.
- Fifth Axiom: The whole is greater than the part.
- First Postulate: To draw a line from any point to any point.
- Second Postulate: To produce a finite straight line continuously in a straight line.
- Third Postulate: To describe a circle with any center and distance.
- Fourth Postulate: That all right angles are equal to one another.
- Fifth Postulate: That, if a straight line falling on two straight lines make the interior angles on the same side less than two right angles, the two straight lines, if produced indefinitely, meet on that side of which are the angles less than the two right angles.

In the modern practice, as in Hilbert's geometry, the first principles of any formal deductive system are "axioms," regardless of what we think about their truth -- which in many cases has been a purely conventionalistic attitude. 

1. Axioms of Incidence:
    1. For every two points A, B there exits a line a that contains each of the points A, B.
    2. For every two points A, B there exists no more than one line that contains each of the points A, B.
    3. There exist at least two points on a line. There exist at least three points that do not lie on a line.
    4. For any three points A, B, C that do not lie on the same line there exists a plane [alpha] that contains each of the points A, B, C. For every plane there exists a point which it contains.
    5. For any three points A, B, C that do not lie on one and the same line there exists no more than one plane that contains each of the three points A, B, C.
    6. If two points A, B of a line a lie in a plane [alpha], then every point of a lies in the plane [alpha].
    7. If two planes [alpha], [beta] have a point A in common, then they have at least one more point B in common.
    8. There exist at least four points which do not lie in a plane.
2. Axioms of Order:
    1. If a point B lies between a point A and a point C, then the points A, B, C are three distinct points of a line, and B then also lies between C and A.
    2. For two points A and C, there always exists at lest one point B on the line AC such that C lies between A and B.
    3. Of any three points on a line there exists no more than one that lies between the other two.
    4. Let A, B, C be three points that do not lie on a line and let a be a line in the plane ABC which does not meet any of the points A, B, C. If the line a passes through a point of the segment AB, it also passes through a point of the segment AC, or through a point of the segment BC.
3. Axioms of Congruence:
    1. If A, B are two points on a line a, and A' is a point on the same or on another line a' then it is always possible to find a point B' on a given side of the line a' through A' such that the segment AB is congruent or equal to the segment A'B'. In symbols AB = A'B'.
    2. If a segment A'B' and a segment A"B", are congruent to the same segment AB, then the segment A'B' is also congruent to the segment A"B", or briefly, if two segments are congruent to a third one they are congruent to each other.
    3. On the line a let AB and BC be two segments which except for B have no point in common. Furthermore, on the same or on another line a' let A'B' and B'C' be two segments which except for B' also have no point in common. In the case, if AB = A'B' and BC = B'C' then AC = A'C'.
    4. Let angle(h,k) be an angle in a plane [alpha] and a' a line in a plane [alpha]' and let a definite side of a' in [alpha]' be given. Let h' be a ray on the line a' that emanates from the point O'. Then there exists in the plane [alpha]' one and only one ray k' such that the angle(h,k) is congruent or equal to the angle(h',k') and at the same time all interior point of the angle(h',k') lie on the given side of a'. Symbolically angle(h,k) = angle(h',k'). Every angle is congruent to itself, i.e., angle(h,k) = angle(h,k) is always true.
    5. If for two triangles ABC and A'B'C' the congruences AB = A'B', AC = A'C', angleBAC = angleB'A'C' hold, then the congruence angleABC = angleA'B'C' is also satisfied.
4. Axiom of Parallels:
    1. (Euclid's Axiom) Let a be any line and A a point not on it. Then there is at most one line in the plane, determined by a and A, that passes through A and does not intersect a.
5. Axioms of Continuity:
    1. (Archimedes' Axiom or Axiom of Measure) If AB and CD are any segments, then there exists a number n such that n segments CD constructed contiguously from A, along the ray from A through B, will pass beyond the point B.
    2. (Axiom of Line Completeness) An extension of a set of points on a line with its order and congruence relations that would preserve the relations existing among the original elements as well as the fundamental properties of line order and congruence that follow from Axioms I-III, and from V,1 is impossible.
    
Given Kant's view of geometry, however, the Euclidean distinction could be restored:  "axioms" would be analytic propositions, and "postulates" synthetic. Whether any of Euclid's original axioms are analytic is a good question. We can see that Hilbert's axiomatic system is logically a much more rigorous system than Euclid's.

### Zermelo-Fraenkel Axiomatic System

The axiomatic system of set theory as we know it today was in large part developed in the period of 1908 to 1922 by Enst Zermelo and Abraham Fraenkel to formulate a theory of sets free of the paradoxes such as Russel's paradox. Mathematicians T. Skolem and John von Neumann made slight modifications to these a few years later.

Zermelo-Fraenkel set theory intended to formalize a single primitive notion, that of a hereditary well-defined set, so that all entities in the universe of discourse are such sets. Thus, the axioms of Zermelo-Fraenkel set theory refer only to pure sets and prevents its models from containing urelements, elements of sets that are not themselves sets. Furthermore, proper classes can only be indirectly. Specifically, Zermelo–Fraenkel set theory does not allow for the existence of a universal set (a set containing all sets) nor for unrestricted comprehension, thereby avoiding Russell's paradox. Von Neumann–Bernays–Gödel set theory (NBG) is a commonly used conservative extension of Zermelo–Fraenkel set theory that does allow explicit treatment of proper classes.

There are many equivalent formulations of the axioms of Zermelo–Fraenkel set theory. Most of the axioms state the existence of particular sets defined from other sets. For example, the axiom of pairing says that given any two sets $a$ and $b$ there is a new set $a,b$ containing exactly $a$ and $b$. Other axioms describe properties of set membership. A goal of the axioms is that each axiom should be true if interpreted as a statement about the collection of all sets in the von Neumann universe (also known as the cumulative hierarchy).

The metamathematics of Zermelo–Fraenkel set theory has been extensively studied. Landmark results in this area established the logical independence of the axiom of choice from the remaining ZFC axioms and of the continuum hypothesis from ZFC. The consistency of a theory such as ZFC cannot be proved within the theory itself, as shown by Gödel's second incompleteness theorem.

Formally, ZFC is a one-sorted theory in first-order logic. The signature has equality and a single primitive binary relation, set membership, which is usually denoted $\in$. The formula $a \in b$ means that the set $a$ is a member of the set $b$ (which is also read, "$a$ is an element of $b$" or "$a$ is in $b$").

### Primitive concepts and notation

What makes a set of primitive concepts and axioms suitable for a particular theory? Most will agree that these must satisfy the following conditions:

1. The number of undefined terms and axioms must be as few as possible
2. Normally, an axiom should not be logically deducible from other axioms, otherwise it will no longer be atomic
3. We should be able to prove from these axioms and concepts most of what we consider to be of interest or useful mathematics. Often, parts of the logical universe which is determined from the axioms are preconceived, in the sense that axioms are introduced so that certain mathematical statements will turn out to be true.
4. These axioms must not lead to any paradoxes. An axiomatic system which contains contradictions is either modified to one in which these contradictions do not occur or some axioms are simply discarded and replaced with others if needed.

The primitive concepts in our theory. There will be three undefined notions in our axiomatic system. They are the words: "class", "set", and "belongs to". The expression "belongs to" is often stated as "is a member of" or "is an element of"; it is usually abbreviated by the symbol, $\in$.

All objects in our theory are classes. There is nothing else. We will soon distinguish special kinds of classes. Once we have discussed a few axioms, we will define a set as being a special kind of class. A class which is not a set will be called a proper class. Some axioms will help us distinguish between those classes which are sets and those which are proper classes. Classes will be represented either lower-case or upper-case letters. So we can write "Let $x$ and $A$ be two classes".

The expression "$x \in A$" is to be read as "the class $x$ belongs to class $A$", or "the class $x$ is in the class $A$" or "$x$ is an element of $A$". However, no class will be representable by a lower-case letter, $x$, unless it is known that $x in B$ for some class $B$. Those classes which can be represented by a lower-case letter, say x, will be given a special name:

> If a class A is such that $A \in B$ for some classes $B$, then we will refer to the class $A$ as being an "element"

Elements are still classes; but they are special classes, since they "belong to" another class. So an element can be represented by both a lower-case or an upper-case letter. For example, if we write $x \in y$ or $A \in B$ this means that $x, y$ and $A$ are elements while $B$ may or may not be an element.

Why is "element" not an undefined notion? It may be surprising that the object element is not expressed as an undefined notion. After all, we are accustomed to distinguishing an element from a set. Introducing a fourth undefined term was eventually seen as superfluous. Consider:

- points $(a, b)$ in the Cartesian plane are actually two-element sets $\{a, b\}$ of real numbers stated in a particular order.
- rational numbers $a/b$ can be described as the set of all two-element sets $\{a, b\}$ of integers in a particular order where $b \ne 0$.
- irrational numbers can be viewed as infinite sequences of rational numbers converging to a non-rational number, again a set

### Axiomatic Set Theory

These are called the ZF axioms. At this point, much of these will look like gibberish but as we progress, we will step by step develop a better understanding of whaat they mean.

**Primitive Concepts**: "class", "set", "belongs to"

1. Axiom of Extent: For the classes $x, A \text{ and } B, [A=B] \Leftrightarrow [x \in A \Leftrightarrow x \in B]$. This states that a class is defined by its elements. If two classes are equal, then they have the same elements. Conversely, two classes which have the same elements are the same class.
2. Axiom of Class Construction: Let $P(x)$ designate a statement about $x$ which can be expressed entirely in terms of the symbols $\in$, $\lor$, $\land$, $\neg$, $\Rightarrow$, $\forall$, brackets and variables $x, y, z, ..., A, B, ...$ Then there exists a class $C$ which consists of all the elements $x$ which satisfy $P(x)$. This states that we can use well-defined properties which can be expressed by the given symbols to construct classes. For example $A = \{ X : u \in X \}$ and $B = \{ X:X = X \}$ are different classes since the properties that characterize their elements are different. For the class $A, P(x)$ is the property $u \in X$ while for the class $B, P(x)$ is the property $X = X$.
3. Axiom of Pair: If $A$ and $B$ are sets, then the doubleton $\{A, B\}$ is a set.
4. Axiom of Subsets: If $S$ is a set and $\phi$ is a formula describing a particular property, then the class of all sets in $S$ which satisfy this property $\phi$ is a set. More succinctly, every subclass of a set of sets is a set. This is more often expressed as the Axiom of Comprehension, Axiom of Specification or the Axiom of Separation. IT is in fact many axioms (which, when viewed together, are referred to as a schema) each differing only by the formula $\phi$ it refers to. So to be more precise, given a formula $\phi$ in set theory language, we would refer to it as axiom $A4(\phi)$ rather than $A4$.
5. Axiom of Power Set: If $A$ is a set, then the power set $\mathscr{P}(A)$ is a set.
6. Axiom of Union: If $\mathscr{A}$ is a set of sets, then $\bigcup_{C \in \mathscr{A}}C$ is a set.
7. Axiom of Replacement: Let $A$ be a set. Let $\phi(x, y)$ be a formula which associates to each element $x$ of $A$ an element $y$ in such a way that whenever both $\phi(x, y)$ and $\phi(x, z)$ hold true, $y = z$. Then there exists a set $B$ which contains all elements $y$ such that $\phi(x, y)$ holds true for some $x \in A^2$. This axiom is more often expressed as the Replacement Axiom Schema since it is in fact many axioms each differing only by the formula $\phi$. And like axiom of subsets, to be more precise, this is referred to as $A7(\phi)$ rather than $A7$.  It essentially allows us to confirm that if the domain $A$ of a set $f$ is a set, then the image $f[A]$ is a set.
8. Axiom of Infinity: There exists a non-empty class $A$ called a set that satisfies the condition: "$X\in A$" $\Rightarrow$ "$X \cup \{X\} \in A$". It says that there exists a class called a set which is infinite in size. This axiom also guarantees that at least one class called a set exists. It essentially allows us to define the "natural numbers", 0, 1, 2, 3, 4, ...
9. Axiom of Regularity: Every non-empty set $A$ contains an element $x$ whose intersection with $A$ is empty.

Notes:

- Axioms 1 and 2 refer only to classese while all the other axioms are "set axioms". The set axioms determine what kind of objects exist in the universe of all sets. 
- Axioms A2 to A7 are constructive axioms. A2 gives us a way to construct a class by referring to a property. Axioms A3 to A7 provide a method to construct new sets from ones that are known to exist. Axiom 
- Axiom 9 is sometimes referred to as the useless axiom. Others don't consider it as a basic axiom since most mathematics which is based on set theory does not require it. However, although it is not obvious, this axiom states that "those empty classes which dont have a least element are not sets". It is in fact an axiom that does not allow certain types of sets to exist in the universe of sets. It is of an exclusionary nature. The other axioms except A1 increase the number of sets in the universe of sets.

### Axiom of Choice

Another special axiom is usually stated separately from the other nine axioms above. It is viewed by many as being different in nature. It was also quite controversial.

Axiom of Choice: For every set $\mathscr{A}$ of non-empty sets, there is a function $f$ which associates to every set $A$ in $\mathscr{A}$ an element $a \in A$.

The controversy surrounding the Axiom of Choice requires some explanation. The axiom of choice is an axiom which was added after most of the ZF axioms were widely accepted as a foundation for modern mathematics. It is so subtle a concept that many early mathematicians unknowingly invoked it in their proofs. Stating it explicitly as an assumption. Some mathematicians publicly questioned this assumption, asking openly whether the word "obviously" was sufficient justification for using it. 

These questions could not be ignored and numerous attempts to derive the axiom of choice from the other ZF axioms failed. In 1963, it was finally proven that neither the Axiom of Choice nor its negation can be proven from the ZF-axioms. This implies that we are free to state it as an axiom along with other ZF axioms, without fear of contradiction. 

A lengthy debate then followed on whether this statement should be included in the fundamental axioms. Some described it as the most interesting in spite of its late appearance and the most discussed axiom of mathematics second only to Euclid's axiom of parallels which was introduced a thousand years ago. Eventually, it was felt that not accepting the Axiom of Choice closes the door to many fundamentally important results of modern mathematics. One could say that the axiom of choice had already been used so extensively that it was deeply ingrained in the modern mathematical fabric.

Even though proofs that invoke the Axiom of Choice were widely viewed as acceptable, it was often felt that the correct proof that does not invoke the Axiom of Choice is preferable to a simpler proof which invokes it. This is because it assumes the existence of something that can neither be seen nor constructed. It is regarded somewhat like some sort of magic wand that magical opens closed doors. For this reason, when proving a statement, it is customary to point out explicitly the steps where the Axiom of Choice is invoked.

There is however one consensus regarding the Axiom of Choice - that it should not be listed together with the other axioms and should be in a category of its own. Together, these nine axioms and the axiom of choice is known as "ZF + Choice" or ZFC. 

## Concept Review: 

1. What is Russel's Paradox?
2. Why do paradoxes occur?
3. What are the three primitive concepts of set theory?
4. What is the difference between a class, a set and a proper class?
5. When is a class called an element?
6. Which classes can be represented by lower case letter?
7. What does ZFC stand for?
8. How many axioms belong to ZFC?