# Previous
[Statistical Inference](3%20-%20statistical%20inference.md)

# Definitions
- The `probability` of an event is defined as the proportion of times this event occurs in many repetitions.
- `A` and `B` are mutually exclusive if they cannot occur at the same time.
- `A` and `B` are independent if knowing the occurrence of one does not change the probability that the other one occurs.

## Four Rules
- Complement: $P(A\text{ does not occur}) = 1 - P(A)$
- Equally likely outcomes: if there are n possible and equally likely outcomes, then $P(A) = \frac{\text{number of outcomes in }A}{n}$
- Addition: If `A` and `B` are mutually exclusive, then $P(A\text{ or }B) = P(A) + P(B)$
- Multiplication: If `A` and `B` are independent, then $P(A\text{ and }B) = P(A)P(B)$

## Conditional Probability
The conditional probability of `B` given `A`:
$$P(B|A) = \frac{P(A \text{ and } B)}{P(A)}$$

So the generalized multiplication rule would be:
$$P(A \text{ and } B) = P(A)P(B|A)$$

if `A` and `B` are independent then by definition $P(B|A) = P(A)$

## Bayes' Rule
$$P(B|A) = \frac{P(A|B)P(B)}{P(A)}$$

Definition of **prior** and **posterior** probabilities. The change of probability after knowing the occurrence of an event using bayesian analysis.

## Warner's randomized response model
Suppose we wan't to know what percentage of students have cheated during an exam or not. The problem is they might not answer truthfully if asked directly. We can design an experiment like this: Ask each student to toss two coins and provide these questions:
1. Have you cheated on the exam?
2. Did you get `tails` on the second toss?

Ask the students to write the answer to `Q1` if they got `heads` on the first toss and answer `Q2` otherwise. This way we can calculate the probability of students cheating using bayes' rule without being able to know if any individual has cheated or not.

# Next
[Normal Approximation](./5%20-%20normal%20approximation.md)