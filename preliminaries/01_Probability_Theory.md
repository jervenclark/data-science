# Probability Theory

## History

The concepts of chance and uncertainty have been with us since the start of civilization. People needed to have some sort of system to cope with the uncertainties of the elements, especially the weather because it directly affects their food supply and survival. But it wasn't until the sixteenth century when attempts to analyze games of chance that the modern mathematical theory of probability took its form which was then later built upon by mathematicians like Pierre de Fermat and Blaise Pascal with their works on deriving exact probabilities for certain gambling problems involving dice.

Since then, the theory of probability has steadily developed and has been widely incorporated and applied in diverse fields of studies. Today, probability theory is an important tool in most engineering fields, science, management, and even finance. Researchers are actively engaged in the discovery and establishment of new applications of probability in fields like medicine, meteorology, genetics, law and especially data science and artificial intelligence.

## Probability vs Statistics
We often use the words “probability” and “statistics” together, but do they mean the same thing?

Probability and statistics are closely related branches of mathematics that deals with uncertainties, relative frequencies of events as well as their implications. However, there are fundamental differences between the two. For starters: probability deals with the likelihood that a certain event happens in the future while statistics analyze the frequency of past events. Probability is often regarded as the theoretical branch of mathematics which studies the consequences of mathematical definitions in contrast to statistics which is an applied branch of mathematics which tries to make sense of observations in the real world.

To illustrate, suppose you toss a coin 10 times, what is the likelihood that the result is H all the time? That is a probability. And we can get a single value for this because of a standard computation strategy.

Now, suppose you want to know if the coin you are using is fair. To do so, you toss it 100 times and count the number of heads. Statistics then is used to draw a conclusion (inference) from this data.

Our goal is to build a mathematical framework to represent and analyze uncertain phenomena such as the result of tossing a coin, weather forecast, the result of a sports competition, etc. We model the phenomenon of interest as an experiment with several, and sometimes potentially infinite, set of mutually exclusive outcomes.

Except maybe for simple cases, when the number of events is small, it is customary to reason about sets of outcomes. To quantify how likely it is for the outcome of an experiment to belong to a specific event, we assign a probability to the event. More formally, we define a measure, a function that maps sets to real numbers, that assigns probabilities to each event of interest. The experiment then is characterized by constructing a probability space.

## Interpretations of Probability

The concept of probability is very pervasive even in everyday life and conversations. Statements like “it probably will rain tomorrow afternoon”, “it is highly unlikely that she will come on time” or “chances are he will fail the finals”. Each of these expressions is based on the concepts of probability and the likelihood of the occurrence of some specific event. But even so, there is no single scientific interpretation of the term probability that is accepted by all statisticians, philosophers and other authorities. In fact, even the true meaning of probability is still a highly controversial subject. Does probability measure the real, physical tendencies of something occurring or is it a measure of how strongly we believe it will occur?

### Classical Interpretation

The classical interpretation of probability is based on the concept of equally likely outcomes which has been championed by Pierre-Simon Laplace developed from studies of games of chances. For example, tossing a fair coin. There are two possible outcomes: head or tail. If it may be assumed that these have an equal likelihood of occurring, then they must have the same probabilities. And, since the sum of the probabilities must be equal to 1, then both probabilities must have ½ chances. Generally, if the outcome of some process must be of n different outcomes and each of these outcomes are equally likely, then the probability of each outcome is 1/n. 

One clear limitation for the classical interpretation is that we can only apply this to situations where there is a finite number of equally possible outcomes. Ther is also no systematic method for assigning probabilities to outcomes that are not assumed to be equal. And second, the concept of equally likely outcomes is essentially based on the concept of probability which we are trying to define. The statements that two possible outcomes are equally likely to occur is the same as the statement that two outcomes have the same probability.

Aside from the classical interpretation, there are currently two broad categories of probability interpretations which can be called evidential and physical probabilities. Each of these interpretations can be very useful when applied to different practical problems. 


### Frequency Interpretation

Frequentists proposes that the probability of an event is its relative frequency over time. Meaning, the probability that some specific outcome of a process will be obtained can be interpreted to mean the relative frequency with which that outcome would be obtained if the process were repeated a large number of times under the same conditions. This is known as aleatory probability.

These events are assumed to governed by some random physical phenomena which are either predictable, in principle, with sufficient information or phenomena that are essentially unpredictable.

For example, the tossing a fair coin, frequentists say that the probability of obtaining a head when a coin is tossed is considered to be ½ not because there are two outcomes but because repeated series of large numbers of trials demonstrate that the empirical frequency converges to the limit ½ as the number of trials goes to infinity.

Of course, the conditions mentioned in this example are too vague to serve as the basis for a scientific definition of probability. It is, of course, impossible to actually perform an infinite repetition of a random experiment to determine the probability of an event. If, however, we only do a finite number of repetitions, we will then have different relative frequencies across different series of trials. 

It is also stated that the relative frequency of heads is approximately ½, but no limit is specified for the permissible variation from ½. If a coin were tossed a million times, we expect to be very near 500,000. On the other hand, we would be very surprised if we obtain exactly 500,000 heads. It would be desirable to be able to make a precise statement of the likelihoods of the different possible numbers of heads, but this error of measurement attached can only be expressed as a probability which is the very concept that we are trying to define.

Another shortcoming of the frequency interpretation of probability is that it only applies to problems in which there can be at least in principle, be a large number of similar repetitions of a certain process. Many important problems are not of this type. For example, the frequency interpretation cannot be applied to the probability that a specific acquaintance will get married within the next two years or to the probability that particular medical research will succeed in coming up with a vaccine for a certain illness within a certain period of time.


### Subjective Interpretation

According to the subjective interpretation of probability, the probability that a person assigns a possible outcome to a certain process represents her own judgment of the likelihood that the outcome will be obtained. It gives the notion of probability as subjective status by regarding it as a measure of the degree of belief of the individual assessing the uncertainty of a particular situation. Another person, who may have different beliefs or different information, may assign a different probability to the same outcome. For this reason, it is appropriate to speak of a certain person’s subjective probability of an outcome, rather than speak of the true probability of the outcome. To illustrate, suppose that a coin is to be tossed once. A person with no special information about the coin or the way in which it is tossed might regard a head or tail probability of ½ and assign a subjective probability of ½ to the possibility of obtaining a head. The person who is actually tossing the coin, however, might feel a little different in that a head is a more likely result. In or that people, in general, may be able to assign subjective probabilities to the outcomes, they must express the strength of their belief in numerical terms. 

This subjective interpretation of probability can be formalized. In general, if people’s judgment of the relative likelihoods of various combinations of outcomes satisfies certain conditions of consistency, then it can be shown that their subjective probabilities of the different possible events can be uniquely determined. 

This, however, is problematic. The requirement that a person’s judgments of the relative likelihoods of an infinite number of events be completely consistent and free from contradictions does not seem to be humanly attainable unless a person is simply willing to adopt a collection of judgments known to be consistent. Also, the subjective interpretation of provides no “objective” basis for two or more scientists working together to reach a common evaluation of the state of knowledge in some scientific area of interest.

## Experiments and Events

In the context of probability, an experiment (or a trial) is any process, real or hypothetical, that can be repeated an infinite number of times and has a well-defined set of possible outcomes that can be determined ahead of time, known as the sample space. An experiment is said to be random if it has more than one outcome otherwise, it is deterministic. A random experiment that has exactly two mutually exclusive possible outcomes, however, is known as a Bernoulli trial. Moreover, the theory of probability pertains to the various possible outcomes that might be obtained and the possible events that might occur when an experiment is conducted.

When an experiment is performed, one and only one outcome results. After repeating the experiment and pooling the results, an experimenter can then obtain an empirical assessment of the probabilities of the various outcomes and events that occur in the experiment.

This definition allows us to call almost any imaginable process an experiment, whether or not its outcome will ever be known. The probability of each event will be our way of saying how likely it is that the outcome of the experiment is in the event. Not every set of possible outcomes will be called an event.

## Mathematical Probability Theory

### Definition: Probability Space

A probability space is a mathematical triplet $(\Omega, \mathcal{F}, P)$ that represents a model for a particular class fo real-world situation. It consists of three elements:
- A sample space $\Omega$, is an arbitratry, non-empty set which contains all possible outcomes for the experiment.
- A $\sigma$-algebra $\mathcal{F} \subseteq 2^{\Omega}$ (called a $\sigma$-field), is a set of subsets of $\Omega$ such that:
  - $\mathcal{F}$ contains the sample space: $\Omega \in \mathcal{F}$,
  - $\mathcal{F}$ is closed under complements: if $A \in \mathcal{F}$, then also $(\Omega \setminus A) \in \mathcal{F}$
  - $\mathcal{F}$ is closed under countable unions: if $A_i \in \mathcal{F}$, for $i = 1,2,3, ...$ then also $(\Omega \setminus A) \in \mathcal{F}$
- A probability measure $P : \mathcal{F} \to [0, 1] $, is a function that assigns probabilities to events in $\mathcal{F}$ such that:
  - $P$ is countably additive (also $\sigma$-additive): if $\{ A_i \}_{i=1}^{\infty} \subseteq \mathcal{F}$ is a countable collection of pairwise disjoint sets, then $ P(\bigcup_{i=1}^{\infty} A_i) = \sum_{i=1}^{\infty} P(A_i) $,
  - the measure of entire sample space is equal to one: $P(\Omega) = 1$

Sample spaces may be discrete or continuous. Examples of discrete sample spaces include possible outcomes of a coin toss, a game score, the number of people that show up at a party, etc. Continuous sample spaces are usually intervals of $\mathbb{R}$ or $\mathbb{R}^n$ used to model time, position, temperature, etc.

We can associate a probability space $(\Omega, \mathcal{F}, P)$ with any experiment, and all questions associated with the experiment can be reformulated in terms of this space. It may seem natural to ask for the numerical value of the probability $P(A)$ of an event $A$. The answer to such a question must be contained in the description of the experiment in question.

A probability space $(\Omega, \mathcal{F}, P)$ is said to be complete probability space if for all $B \in \mathcal{F} \text{ with } P(B) = 0$ and aall $A \subset B$ one has $A \in \mathcal{F}$.

#### Discrete Case

Discrete probability theory needs only at most countable sample spaces $\Omega$. Probabilities can be ascribed to points of $\Omega$ by the probability mass function $p : \Omega \to [0, 1]$ such that $\sum_{ \omega \in \Omega} p(\omega) = 1$. All subsets of $\Omega$ can be treated as events (thus, $\mathcal{F} = 2^{\Omega}$ is the power set). The probability measure takes the simple form

$$ 
P(A) = \sum_{\omega \in A} p(\omega) \text{ for all A} \subseteq \Omega
$$

The greatest $\sigma$-algebra $\mathcal{F} = 2^{\Omega} $ describes the complete information. In general, a $sigma$-algebra $\mathcal{F} \subseteq 2^{\Omega}$ corresponds to a finiite or countable partition $\Omega = B_1 \cup B_2\ \cup ...$, the general for of an event $A \in \mathcal{F}$ being $A = B_{k_1} \cup B_{k_2} \cup ...$. The case $p(\omega) = 0$ is permitted but rarely used because $\omega$ can safely be excluded from the sample space.

#### General Case

If $\Omega$ is uncountable, still, it may happen that $p(\omega) \neq 0$ for some $\omega$; such $\omega$ are called atoms. They are an at most countable set, whose probability is the sum of probabilities of all atoms. If this sum is equal to 1 then all other points can safely be excluded from the sample space, returning us to the discrete case. Otherwise, if the sum is between 0 and 1, then the probability space decomposes into a discrete (atomic) part and a non-atomic part

#### Non-Atomic Case

If $p(\omega) = 0$ for all $\omega \in \Omega$, then equation fails: the probability of a set is not necessarily the sum over the probabilities of its elements, as summation is only defined for countable numbers of elements. This makes the probability theory much more technical and a formulation stronger than summation, measure theory is applicable. Initially, the probabilities are ascribed to some generator sets. Then a limiting procedure allows assigning probabilities to set that are limits of sequences of generator sets, or limits of limits, and so on. All these sets are the $\sigma$-algebra $\mathcal{F}$. 

In each experiment, it is necessary to assign to each event $A$ in the sample space $S$ a number $P(A)$ that indicates the probability that $A$ will occur. In order to satisfy the mathematical definition of probability, the number P(A) that is assigned must satisfy three specific axioms:

### Axiom 1: Non-negativity of Probability Measure

For every event $A$, $P(A) \geq 0$. It means that the probability of every event must be non-negative.

### Axiom 2: Probability of Sample Space

$P(S) = 1$. If an event is certain to occur, then the probability of that event is 1.

The first two axioms capture the intuitive idea that the probability of an event is a measure of mass: just like the mass of any object is non-negative and the total mass of several distinct objects is the sum of their masses, the probability of any event is non-negative and the probability of the union of several disjoint objects is the sum of their probabilities. However, in contrast to mass, the amount of probability in an experiment cannot be unbounded. 

### Axiom 3: $\sigma$-additivity

If the sets $A_1, A_2, ..., A_n \in \mathcal{F}$ are disjoint (i.e. $A_i \cap A_j = \emptyset\ for\ i \neq j$) then:

$$ P(\bigcup_{i=1}^n A_i) = \sum_{i=1}^{n}P(A_i) $$

Similarly, for a countably infinite sequence of disjoint sets $A_1, A_2, ... \in \mathcal{F}$

$$P(\lim_{n \to \infty } \cup_{i=1}^n A_i) = \lim_{n \to \infty } \sum_{i=1}^{n}P(A_i)$$

To put the third axiom into perspective, if two events are disjoint, it is natural to assume that the probability that one or the other will occur is the sum of their individual probabilities. In fact, it will be assumed that this additive property of probability is true for every finite collection of disjoint events and even for every infinite sequence of disjoint events.

### Example: Tossing a Coin

For example, suppose we have an event $A$ for when tossing a coin, you get two possible results: $H$ or $T$, so the sample space is $\Omega = \{H, T\}$ and $\mathcal{F} = \{ \{H, T\}, H, T, \emptyset \}$ and a possible probability measure $P: \mathcal{F} \to [0,1]$ is given by:

- $P(\emptyset) = 0$,
- $P(H) = p$,
- $P(T) = 1 -p $,
- $P(\Omega) = 1$

An event $E$ is a set of zero or more outcomes, i.e., a subset of the sample space and valid $E$ are:

- $\{H,T\} \subset \Omega$
- $\{ H \} \subset \Omega$
- $\emptyset \subset \Omega$

An event is considered to have happened during an experiment when the outcome of the latter is an element of the event. Since the same outcome may be a member of many events, it is possible for many events to have happened given a single outcome. 

For each subset $A$ of $\Omega$, let $P(A)$ be the number of elements of $A$ divided by $|\Omega|$. It is trivial to see that these satisfies the first 2 axioms. There are only finitely many distinct collections of nonempty disjoint events which also satisfies the 3rd axiom.

### Definition: $\sigma$-algebra

A $\sigma$-algebra $\mathcal{F}$ is a collection of sets in $\Omega$ such that:

1. If a set $A \in \mathcal{F}$ then $A^c \in \mathcal{F}$
2. If the sets $A_1, A_2 \in \mathcal{F}$, then $A_1 \cup A_2 \in \mathcal{F}$. This also holds for infinite sequences; if $A_1, A_2, ... \in \mathcal{F} $ then $ \cup_{i=1}^{\infty}A_i \in \mathcal{F}$
3. $\Omega \in \mathcal{F}$

The smallest $\sigma$-field is the collection $\mathcal{F} = \{ \emptyset, \Omega \}$. If our sample space is discrete, a possible choice for the $\sigma$-algebra is the power setof the sample space, which consists of all possible sets of elements in the sample space. If we are tossing a coin and the sample space is  $ \Omega := \{ H, T \} $ then the power set is a valid $\sigma$-algebra $ \mathcal{F} := \{ \{H,T\},\ H,\ T,\ \emptyset \} $, where $\emptyset$ denotes the empty set. 

However, in many cases, $\sigma$-algebras do not contain every possible set of outcomes. Suppose that the sample space $\Omega = \{ \omega_1, ...,\omega_n \}$ is finite. If $\Omega$ is finite and if each outcome is equally likely, then $ P(A) = \frac{|A|}{\Omega} $ which is called a uniform probability distribution. to compute probabilities, we need to count the number of points in an event $A$. Methods for counting points are called combinatorial methods.

Given $n$ objects, the number of ways of ordering these objects is $n! = n(n-1)(n-2)...3\cdot 2\cdot 1$. We also define

$ {n \choose k} = \frac{n!}{k!(n-k)!} $

read as "n choose k", which is the number of distinct ways of choosing k objects from n. For example, if we have a class of 20 people and we want to select a committee of 4 people, then there are

$ \begin{align} {n \choose k} &= \frac{n!}{k!(n-k)!} \\&= \frac{20!}{4!16!} \\&= \frac{20 \times 19 \times 18 \times 17}{4 \times 3 \times 2 \times 1} \\&= 174420 \end{align}$

possible commitees. We note the following properties:

$ \begin{align} {n \choose 0} &= {n \choose n} = 1
\\ {n \choose k} &= {n \choose n-k } \end{align}$

### Example: Throwing a Loaded Die

There are other choices for the probabilities of events. For instance, if we believe that the die is loaded, we might believe that some sidese have different probabilities of turning up. To be specific, suppose that we believe that 6 is twice as likely to come up as the other five sides. We could set $p_i = \frac{1}{7} $ for $i = 1,2,3,4,5$ and $p_6 = \frac{2}{7}$. Then for each event $A$, we define P(A) to be the sum of all $p_i$ such that $i \in A$. For example, if $A = \{ 1, 3, 5\}$, then $P(A) = p_1 + p_3 + p_5 = \frac{3}{7}$. It is not difficult to verify that these also satisfies the three axioms.

### Definition: Probability Measure

A probability measure, or simply, a probability, on a sample space $\Omega$ is a specification of numbers $P(A)$ for all events $A$ that satisfy Axioms 1, 2, and 3.

The role of the probability measure $P$ is to quantify how likely we are to encounter each of the events in the $\sigma$-algebra. Intuitively, the probability of an event A can be interpreted as the fraction of times that the outcome of the experiment is in A, as the number of repetitions tends to infinity. It follows that the probabilities should always be non-negative. 

### Theorem: $P(\emptyset) = 0$

If an event is impossible, its probability must be 0.

*Proof.* Consider the infinite sequence of events $A_1, A_2, ...$ such that $A_i = \emptyset$ for $i = 1, 2, ...$. In other words, each of the events ini the sequence is just the empty set. Then this sequence is a sequence of disjoint events since $\emptyset \cap \emptyset = \emptyset$. Furthermore, $\bigcup_{i=1}^{\infty} A_i = \emptyset$. 

Therefore, it follows from axiom 3 that

$$
P(\emptyset) = P(\bigcup_{i=1}^{\infty} A_i) = \sum_{i=1}^{\infty}P(A_i) = \sum_{i=1}^{\infty}P(\emptyset)
$$

This states that when the $P(\emptyset)$ is added repeatedly in an infinite series, the sum of that series is simply the number of $P(\emptyset)$ and the only real number with this property is zero.