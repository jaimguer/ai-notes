
# Quantifying Uncertainty

## Acting Under Uncertainty

### Why are agents uncertain?
1. Nondeterminism in the world, and in their behavior
-. Partial observability of the world.  If the agent can't see what is going
on, the agent can't think about its actions.

### How do agents deal with their uncertainty?
Most agents keep around a *belief state*, which is a list of all possible
worlds the agent might currently be in.  This works for small problem spaces
but has some issues overall.
1. An agent would need to keep track of *every* possible world, no matter how
   unlikely that world is.
-. Contingency plans the agent might create become exceedingly large as
   a result of not measuring likelihood.
-. Sometimes, there is no promise that any plan will actually acheive the
    agent's goal, but the agent must act regardless.

The agent's goal is always to maximize its performance measure.  To do that,
it must weigh the relative importance of its goals with considerations on the
likelihood it will acheive those goals.  To summarize its uncertainty and make
a rational decision, we use probability theory.

## Basic Probability Notation

Probabilities are about asserting if something will happen, relative to other
events.  Here are some basic definitions.
1. **sample space**: the set of all possible worlds that are under our consideration.
  1. Denoted as $ \Omega $.
  -. Each $ \omega \in \Omega $ gets a probability assigned to it.
  -. $ 0 \leq P(\omega) \leq 1, \forall \omega \in \Omega $.
  -. $\sum_{\omega \in \Omega} P(\omega) = 1 $.
- **events** are sets of possible worlds that satisfy a given property.
  1. The probability of an event is the sum of the probabilities of the events
     satisfying the property.
  -. Example : Given two dice, $ P(roll = 11) = P(5,6) + P(6,5) = \frac{1}{18}$.
- Probabilities of events with no other information are called *priors* or
  *unconditional probabilities*.
- *Posterior (conditional)* probabilities are those probabilities given some
  other piece of information.
- $ P(a \land b) = P (a \vert b) P(b) $. This rearrainges to the more
  familiar fractional equation of conditional probabilities.
- A **probability distribution** of a discrete random variable is a listing of
  the values the random variable can take.



