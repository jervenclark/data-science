# Random Variables

Random variables are fundamental in probabilistic modeling. They allow us to numerically model quantities that are uncertain: temperature tomorrow, time of flight arrival, and so on. Reasoning about such quantities probabilistically allow us to structure information in a principled way.

## Definition

Formally, we define random variables as a function mapping each outcome in a probability space to a real number meaning. For each random variable $X$ and each set $S$ of real numbers, we could calculate the probability that X takes its values from $S$/ The collection of all of these probabilities is the distribution of $X$. There are two major classes of distributions and random variables: discrete and continuous. 

Discrete distribution can be characterized by its probability function, which specifies the probability that the random variable takes each of the different possible values. A random variable with a discrete distribution will be called a discrete random variable.

### Definition: Random Variable

> Given a probability space $(\Omega, \mathcal{F}, P)$, a random variable $X$ is a function from the sample space $\Omega$ to the real numbers $\mathbb{R}$. Once the outcome $\omega \in \Omega$ of the experiment is revealed, the corresponding $X(\omega)$ is known as the realization of the random variable.

### Remark: Rigorous Definition

> Consider two sample spaces $\Omega_1$ and $\Omega_2$, and a $\sigma$-algebra $\mathcal{F}_2$ of sets in $\Omega_2$. Then, for $X$ to be a random variable, there must exist a $\sigma$-algebra $\mathcal{F}_1$ in $\Omega_1$ such that for any set $S \in \mathcal{F}_2$ the inverse image of $S$, defined by
>
> $$ X^{-1} (S) := \{\omega | X(\omega) \in S\},$$
>
> belongs to $\mathcal{F}_1$. Usually, we take $\Omega_2$ to be the reals $\mathbb{R}$ and $\mathcal{F}_2$ to be the Borel $\sigma$-algebra. In any case, for the purpose of notes, the definition is sufficient.

### Remark: Notation

> We often deenote events of the form 
>
> $$\{X(\omega) \in S : \omega \in \Omega\}$$
>
> for some random variable $X$ and some set $S$ as
>
> $$\{X \in S\}$$
>
> to alleviate the notation, since the underlying probability space is often of no significance once we have specified the random variables of interest.

A random variable quantifies our uncertainty about the quantity it represents, not the value that it happens to finally take once the outcome is revealed. You should never think about the random variable as a fixed numerical value. If the outcome is known, then that determines a realization of the random variable. In order to stress the difference between random variables and their realizations, we denote the former with uppercase letters $(X, Y, ...)$ and the latter lowercase letters $(x, y, ...)$

### Example