Lecture 5. Introduction to First Order Logic
============================================

## Recap of Propositional Logic

Thus far in our journey into logic we have seen

1.  **propositions** or "statements," which are sentences that can be judged true or false, and which we denote using variables like A, B, C, and other capital letters.

2.  The **logical connectives** ∧, ∨, →, ¬, which are operations (or functions) that take propositions as inputs and produce new propositions as outputs.

    +  For example, ∧ is a binary operation on propositions: given propositions A and B, we can form A ∧ B which is the proposition "A and B".

    +  Another example, ¬ is a unary operation (since it takes one argument): given a proposition A, we form ¬ A which is the proposition "not A".
   
3.  **Rules of deduction**
    (e.g., the system of "natural deduction," as described in the Logic and Proof book, defines the so-called *introduction* and 
    *elimination rules*, which are listed at the end of these notes for your convenience.)

The system of logic based on 1., 2., and 3. is called **Propositional Logic**.

Propositional Logic is quite useful, but it can only take us so far. Eventually, we will find ourselves in situations where we want 
to write sentences as functions, like P(x), where the truth value of P(x) may depend on the value of x.

For example, P(x) could denote the sentence "At temperature x, water boils."

As it stands, P(x) is *not* a statement because it involves a **free variable**---namely, x.

Sentences with free variables cannot be judged true or false until we are given a value for x.
They may be true for some values of x (e.g., x ≥ 100° C), and false for others (e.g., x < 100° C).

A sentence or function or formula involving free variables, which may be true or false depending on how we assign values to its free variables, is called a **predicate**.

Logic involving predicates, the logical connectives, and rules of deduction is called **Predicate Logic** or **First Order Logic**.


-------------------

## Quantifiers

There are two "quantifiers" in logic, the universal quantifier (∀) and the existential quantifier (∃).

### The Universal Quantifier ∀

The **universal quantifier**, denoted ∀, means "for all."

Example. ∀ x, x ∈ A → x ∈ B  means "for all x, if x is in A, then x is in B."

Note that, if we assume the sets A and B are known, then the formula

∀ x, x ∈ A → x ∈ B

is actually a statement or "proposition" (it can be judged true or false).

It is *not* a predicate because it does not depend on x.

Indeed, it is equivalent to the statement "A is a subset of B", or A ⊆ B,
which clearly does not depend on x.

+  **Question**. What happened to the dependence on x?

+  **Answer**. If we start by letting P(x) denote x ∈ A → x ∈ B, then P(x) is a predicate.

   Its truth value depends on what we pick for x.

   (To see this, let A = {0} and B = {1}. Then, P(x) is false if x = 0 and true otherwise.)
   
   However, as soon as we place the quantifier "∀ x" in front of P(x), the free variable x is "bound" and is no longer free.
   
   Example. ∀ x, P(x)  means ∀ x, x ∈ A → x ∈ B  means A ⊆ B  (which clearly does not depend on x!)
   
   In the statement ∀ x, P(x), there are no free variables, and the x appearing in the formula P(x) 
   is called a *bound variable*, since P(x) appears after the quantifier ∀ x.
   

#### A proof involving the universal quantifier


+  **Claim**. The empty set, denoted ∅, is a subset of every set.

+  **Proof**. Want to show: for any set A, ∅ ⊆ A.

   (Notation. We will use "WTS" to denote the phrase "Want to show".)
       
   Fix some arbitrary set A.  WTS: ∅ ⊆ A; i.e., 

   WTS: ∀ x, x ∈ ∅ → x ∈ A.

   Fix an arbitrary x.  Assume, x ∈ ∅.

   We immediately have a contradiction because ∅ contains no element.

   Therefore, x ∈ ∅ → ⊥, that is, x ∈ ∅ implies False.

   From False, anything follows, in particular, False implies x ∈ A, 
   which was to be shown.

   (Notation. We will often use the abreviation QED for the phrase "which was to be shown."
   Incidentally, QED comes from Latin; it's the acronym of *quid erat demonstrandum*.)


### The Existential Quantifier ∃

The **existential quantifier**, denoted ∃, means "there exists."

We will discuss this more next time, but just like ∀, it can bind free variables and turn predicates into propositions.

We'll see many examples...


-----

## Power sets and cardinalities of sets

### Power set

Given a set X. The collection of all subsets of X
is called the power set of X.

Example. X = {a, b, c}. The lattice of all subsets of X is shown below.


```
             {a, b, c}     ( <-- since X ⊆ X )
            /    |    \
         {a,b} {a,c} {b,c}
           |  \/   \/  |
           |  /\   /\  |
          {a}   {b}  {c}
             \   |   /
                 ∅
```

The collection of all subsets of the set X = {a, b, c} is often written 
down, not as a lattice diagram like the one above, but rather as a set, like this:

𝒫(X) ={ {a, b, c}, {a,b}, {a,c}, {b,c}, {a},  {b},  {c},  ∅ }

A student asked the following:

**Question**. Is {a, b} the same set as {b, a}.  
**Answer**. Yes.


Recall question from homework:

"Is ℕ ∉ 𝒫(ℕ) a statement?"  (Answer given in class.)

### Representing subsets using binary strings.

For a 3 element set, we can represent each subset using a
3-tuple of 0's and 1's.  (x,y,z) <---> {a, b, c}

{a, b, c} <--> (1,1,1)
{a, c} <--> (1,0,1)


### The cardinality or "size" of a set

Cardinality of a set X is a measure of the size of X, and is denoted by |X|.

For finite sets, this is easy to define.  Just count up the number of elements in the set!

**Example**. If X = {a, b, c}, the |X| = 3.

If X is infinite and "countable" or "enumerable" (i.e., we can list all the elements in the set X one-by-one)
then we *define* |X| = ∣ℕ∣.

A fact that is sometimes useful and that we can derive from the observation above (about representing subsets with binary sequences)
is that |𝒫(X)| = 2^|X| (i.e., 2 to the power |X|).

If X is infinite and *uncountable* (i.e., it's impossible to go one-by-one and list the elements 
of the set), then the question "what is the cardinality of X" is more technical and is outside the 
scope of this class.

Example. If ℝ is the set of real numbers, then ∣ℝ| = |𝒫(ℕ)| = 2^|ℕ|.

-----

The rest was covered in an earlier lecture but was not carefully recorded at that time.  (These rules also appear in the Logic and Proof book.)

## Derivation Rules of Natural Deduction

To interpret each of the rules below---in particular, when we want to say one of the rule out loud---we read them as follows: "given the propositions above the horizontal line, we can deduce the proposition below the line."

### Introduction Rules

These tell us how to produce new propositions by using the logical connectives and some "input" propositions that we assume hold.

1.  ∧-introduction rule
    ```
       A   B
      -------
       A ∧ B
    ```
                                     
2.  ∨-introduction rules
    ```
            A             B
         -------       -------
          A ∨ B         A ∨ B
    ```
                                     
3.  →-introduction rule
    ```
       A
       ⋮
       B
     -----
     A → B
    ```
    
4.  ¬-introduction
    ```
      A
      ⋮
      ⊥
    -----
     ¬ A
    ```
    
### Elimination Rules

These tell us how we can make use of (or compute with) each of the forms introduced above.

1.  ∧-elimination rules
    ```
       A ∧ B         A ∧ B
      -------       -------
         A             B
    ```
                                     
2.  ∨-elimination rule
    ```
                   A    B
                   ⋮    ⋮
       A ∨ B       C    C
      ----------------------
                C
    ```

3.  →-elimination rule
    ```
      A → B      A
     --------------
           B
    ```
    
4.  ¬-elimination rule
    ```
      ¬ A  ∧  A
      -----------
           ⊥
    ```
     
