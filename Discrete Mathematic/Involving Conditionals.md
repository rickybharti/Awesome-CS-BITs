### Involving Conditionals

1. **\( p \rightarrow q \equiv \neg q \rightarrow \neg p \) (Contrapositive)**
   - This states that a conditional statement is logically equivalent to its contrapositive.
   - **Truth Table:**
     | \( p \) | \( q \) | \( p \rightarrow q \) | \( \neg p \) | \( \neg q \) | \( \neg q \rightarrow \neg p \) |
     |:---:|:---:|:-------------:|:--------:|:--------:|:------------------------:|
     |  T  |  T  |       T       |    F     |    F     |            T             |
     |  T  |  F  |       F       |    F     |    T     |            F             |
     |  F  |  T  |       T       |    T     |    F     |            T             |
     |  F  |  F  |       T       |    T     |    T     |            T             |

2. **\( (p \rightarrow q) \lor (p \rightarrow r) \equiv p \rightarrow (q \lor r) \)**
   - This states that the disjunction of two conditionals is equivalent to a single conditional with a disjunction in the consequent.
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( p \rightarrow q \) | \( p \rightarrow r \) | \( (p \rightarrow q) \lor (p \rightarrow r) \) | \( q \lor r \) | \( p \rightarrow (q \lor r) \) |
     |:---:|:---:|:---:|:-------------:|:-------------:|:----------------------------------:|:----------:|:----------------------------:|
     |  T  |  T  |  T  |       T       |       T       |                T                 |     T      |              T               |
     |  T  |  T  |  F  |       T       |       F       |                T                 |     T      |              T               |
     |  T  |  F  |  T  |       F       |       T       |                T                 |     T      |              T               |
     |  T  |  F  |  F  |       F       |       F       |                F                 |     F      |              F               |
     |  F  |  T  |  T  |       T       |       T       |                T                 |     T      |              T               |
     |  F  |  T  |  F  |       T       |       T       |                T                 |     T      |              T               |
     |  F  |  F  |  T  |       T       |       T       |                T                 |     T      |              T               |
     |  F  |  F  |  F  |       T       |       T       |                T                 |     F      |              T               |

3. **\( (p \rightarrow r) \lor (q \rightarrow r) \equiv (p \land q) \rightarrow r \)**
   - This states that the disjunction of two conditionals is equivalent to a single conditional with a conjunction in the antecedent.
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( p \rightarrow r \) | \( q \rightarrow r \) | \( (p \rightarrow r) \lor (q \rightarrow r) \) | \( p \land q \) | \( (p \land q) \rightarrow r \) |
     |:---:|:---:|:---:|:-------------:|:-------------:|:----------------------------------:|:----------:|:----------------------------:|
     |  T  |  T  |  T  |       T       |       T       |                T                 |     T      |              T               |
     |  T  |  T  |  F  |       F       |       F       |                F                 |     T      |              F               |
     |  T  |  F  |  T  |       T       |       T       |                T                 |     F      |              T               |
     |  T  |  F  |  F  |       F       |       T       |                T                 |     F      |              T               |
     |  F  |  T  |  T  |       T       |       T       |                T                 |     F      |              T               |
     |  F  |  T  |  F  |       T       |       F       |                T                 |     F      |              T               |
     |  F  |  F  |  T  |       T       |       T       |                T                 |     F      |              T               |
     |  F  |  F  |  F  |       T       |       T       |                T                 |     F      |              T               |

### De Morgan’s Laws

1. **\( \neg (p \land q) \equiv \neg p \lor \neg q \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( p \land q \) | \( \neg (p \land q) \) | \( \neg p \) | \( \neg q \) | \( \neg p \lor \neg q \) |
     |:---:|:---:|:---------:|:------------------:|:--------:|:--------:|:-------------------:|
     |  T  |  T  |    T      |         F          |    F     |    F     |         F           |
     |  T  |  F  |    F      |         T          |    F     |    T     |         T           |
     |  F  |  T  |    F      |         T          |    T     |    F     |         T           |
     |  F  |  F  |    F      |         T          |    T     |    T     |         T           |

2. **\( \neg (p \lor q) \equiv \neg p \land \neg q \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( p \lor q \) | \( \neg (p \lor q) \) | \( \neg p \) | \( \neg q \) | \( \neg p \land \neg q \) |
     |:---:|:---:|:---------:|:------------------:|:--------:|:--------:|:--------------------:|
     |  T  |  T  |    T      |         F          |    F     |    F     |          F           |
     |  T  |  F  |    T      |         F          |    F     |    T     |          F           |
     |  F  |  T  |    T      |         F          |    T     |    F     |          F           |
     |  F  |  F  |    F      |         T          |    T     |    T     |          T           |

3. **\( \neg p \lor q \equiv p \rightarrow q \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( \neg p \) | \( \neg p \lor q \) | \( p \rightarrow q \) |
     |:---:|:---:|:--------:|:-----------------:|:----------------:|
     |  T  |  T  |    F     |        T          |        T         |
     |  T  |  F  |    F     |        F          |        F         |
     |  F  |  T  |    T     |        T          |        T         |
     |  F  |  F  |    T     |        T          |        T         |

### Distributivity

1. **\( p \lor (q \land r) \equiv (p \lor q) \land (p \lor r) \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( q \land r \) | \( p \lor (q \land r) \) | \( p \lor q \) | \( p \lor r \) | \( (p \lor q) \land (p \lor r) \) |
     |:---:|:---:|:---:|:-----------:|:-------------------:|:-----------:|:-----------:|:---------------------------:|
     |  T  |  T  |  T  |      T      |         T           |      T      |      T     

 |             T               |
     |  T  |  T  |  F  |      F      |         T           |      T      |      T      |             T               |
     |  T  |  F  |  T  |      F      |         T           |      T      |      T      |             T               |
     |  T  |  F  |  F  |      F      |         T           |      T      |      T      |             T               |
     |  F  |  T  |  T  |      T      |         T           |      T      |      T      |             T               |
     |  F  |  T  |  F  |      F      |         F           |      T      |      F      |             F               |
     |  F  |  F  |  T  |      F      |         F           |      F      |      T      |             F               |
     |  F  |  F  |  F  |      F      |         F           |      F      |      F      |             F               |

2. **\( p \land (q \lor r) \equiv (p \land q) \lor (p \land r) \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( q \lor r \) | \( p \land (q \lor r) \) | \( p \land q \) | \( p \land r \) | \( (p \land q) \lor (p \land r) \) |
     |:---:|:---:|:---:|:-----------:|:--------------------:|:-----------:|:-----------:|:----------------------------:|
     |  T  |  T  |  T  |      T      |          T           |      T      |      T      |              T               |
     |  T  |  T  |  F  |      T      |          T           |      T      |      F      |              T               |
     |  T  |  F  |  T  |      T      |          T           |      F      |      T      |              T               |
     |  T  |  F  |  F  |      F      |          F           |      F      |      F      |              F               |
     |  F  |  T  |  T  |      T      |          F           |      F      |      F      |              F               |
     |  F  |  T  |  F  |      T      |          F           |      F      |      F      |              F               |
     |  F  |  F  |  T  |      T      |          F           |      F      |      F      |              F               |
     |  F  |  F  |  F  |      F      |          F           |      F      |      F      |              F               |

### Associativity

1. **\( p \lor (q \lor r) \equiv (p \lor q) \lor r \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( q \lor r \) | \( p \lor (q \lor r) \) | \( p \lor q \) | \( (p \lor q) \lor r \) |
     |:---:|:---:|:---:|:-----------:|:-------------------:|:-----------:|:-------------------:|
     |  T  |  T  |  T  |      T      |         T           |      T      |         T           |
     |  T  |  T  |  F  |      T      |         T           |      T      |         T           |
     |  T  |  F  |  T  |      T      |         T           |      T      |         T           |
     |  T  |  F  |  F  |      F      |         T           |      T      |         T           |
     |  F  |  T  |  T  |      T      |         T           |      T      |         T           |
     |  F  |  T  |  F  |      T      |         T           |      T      |         T           |
     |  F  |  F  |  T  |      T      |         T           |      F      |         T           |
     |  F  |  F  |  F  |      F      |         F           |      F      |         F           |

2. **\( p \land (q \land r) \equiv (p \land q) \land r \)**
   - **Truth Table:**
     | \( p \) | \( q \) | \( r \) | \( q \land r \) | \( p \land (q \land r) \) | \( p \land q \) | \( (p \land q) \land r \) |
     |:---:|:---:|:---:|:-----------:|:--------------------:|:-----------:|:--------------------:|
     |  T  |  T  |  T  |      T      |          T           |      T      |          T           |
     |  T  |  T  |  F  |      F      |          F           |      T      |          F           |
     |  T  |  F  |  T  |      F      |          F           |      F      |          F           |
     |  T  |  F  |  F  |      F      |          F           |      F      |          F           |
     |  F  |  T  |  T  |      T      |          F           |      F      |          F           |
     |  F  |  T  |  F  |      F      |          F           |      F      |          F           |
     |  F  |  F  |  T  |      F      |          F           |      F      |          F           |
     |  F  |  F  |  F  |      F      |          F           |      F      |          F           |

### Conclusion:
By constructing the truth tables for each equivalence, you can confirm that the propositions on both sides of each equivalence sign have identical truth values for all possible combinations of \( p \), \( q \), and \( r \). Therefore, they are logically equivalent.
