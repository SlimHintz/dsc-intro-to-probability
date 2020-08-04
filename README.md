
# Introduction to Probability

## Introduction

Now that you understand the basics of sets, you'll learn how this knowledge can be used to calculate your first probabilities! In this section, you'll learn how to use sets to create probabilities and you'll learn about the very foundations of probability through the three probability axioms.

## Objectives

You will be able to: 

* Compare experiments, outcomes, and the event space
* Calculate probabilities by using relative frequency of outcomes to event space
* Describe the three axioms of probability
* Describe the addition law of probability

## Experiment and outcomes

Previously, we defined sets and related concepts. Now let's look at the set

 <img src="https://render.githubusercontent.com/render/math?math=S=   \{1,2,3,4,5,6 \}"> , which contains all possible outcomes when throwing a dice.

When you throw a dice once, you can consider this a *random experiment*. The result of this "experiment" is the *outcome*. 

You can then say that:

-  <img src="https://render.githubusercontent.com/render/math?math=S"> defines all the **possible outcomes** when throwing the dice once
-  <img src="https://render.githubusercontent.com/render/math?math=S"> is our Universal set  <img src="https://render.githubusercontent.com/render/math?math= \Omega"> , as seen before


When conducting experiments, you say that your universal set is your **sample space**: it is the universe in which your possible outcomes are listed as elements.

Other examples of sample spaces:
- The number of text messages you send each day:  in this case, S is equal to some number x, with x being a **positive integer**, or mathematically:  <img src="https://render.githubusercontent.com/render/math?math=S =   \{x   \mid x   \in   \mathbb{Z}, x   \geq 0 \}"> 
- The number of hours someone watches TV each day:   <img src="https://render.githubusercontent.com/render/math?math=S =   \{x   \mid x   \in   \mathbb{R}, 0   \leq x   \leq 24   \}"> 

## Event space

Next, let's define event space. The **event space** is a subset of the sample space,  <img src="https://render.githubusercontent.com/render/math?math=E   \subseteq S"> 

For example, the event "throwing a number higher than 4" when throwing a dice would result in an event space  <img src="https://render.githubusercontent.com/render/math?math=E=   \{5,6 \}"> . Throwing an odd number would lead to an event space  <img src="https://render.githubusercontent.com/render/math?math=E=   \{1,3,5 \}"> . 

Summarized, the event space is a collection of events that we *care* about. We say that event  <img src="https://render.githubusercontent.com/render/math?math=E"> happened if the actual outcome after rolling the dice belongs to the predefined event space   <img src="https://render.githubusercontent.com/render/math?math=E"> .

With **sample space** and **event space**, you now understand the two foundational concepts of **probability**. 

Other examples of event spaces based on previously defined sample spaces:

- If you define that the event "low daily number of text messages sent" means 20 or fewer text messages, the event space is defined as:  <img src="https://render.githubusercontent.com/render/math?math=E =   \{x   \mid x   \in   \mathbb{Z}, 0   \leq x   \leq 20   \}"> 
- Binge-watch day:   <img src="https://render.githubusercontent.com/render/math?math=E =   \{x   \mid x   \in   \mathbb{R}, x   \geq 6   \}"> 

## Introduction to probability

### The law of relative frequency

While conducting an endless stream of experiments, the relative frequency by which an event will happen becomes a fixed number. 

Let's denote an event by  <img src="https://render.githubusercontent.com/render/math?math=E"> , and the _probability_ of the event  <img src="https://render.githubusercontent.com/render/math?math=E"> occurring by  <img src="https://render.githubusercontent.com/render/math?math=P(E)"> . Next, let  <img src="https://render.githubusercontent.com/render/math?math=n"> be the number of conducted experiments, and  <img src="https://render.githubusercontent.com/render/math?math=S(n)"> the count of "successful" experiments (i.e. the times that event  <img src="https://render.githubusercontent.com/render/math?math=E"> happened). The formal definition of probability as a relative frequency is given by:

 <img src="https://render.githubusercontent.com/render/math?math=P(E) =   \lim_{n \rightarrow \infty}   \dfrac{S{(n)}}{n}"> 

This is the basis of a frequentist statistical interpretation: an event's probability is the ratio of the positive trials to the total number of trials as we repeat the process infinitely. 

For example, the probability of rolling a 5 on a 6 sided dice is the limit of the successes to trials as the number of trials goes to infinity.


###  Probability axioms

In the early 20th century, Kolmogorov and Von Mises came up with three axioms that further expand on the idea of probability. The three axioms are:

#### 1. Positivity

A probability is always bigger than or equal to 0, or  <img src="https://render.githubusercontent.com/render/math?math=0   \leq P(E)   \leq 1"> 

#### 2. Probability of a certain event

If the event of interest is the sample space, we say that the outcome is a certain event, or  <img src="https://render.githubusercontent.com/render/math?math=P(S) = 1"> 

#### 3. Additivity 

The probability of the union of two exclusive events is equal to the sum of the probabilities of the individual events happening.

If  <img src="https://render.githubusercontent.com/render/math?math=A    \cap B =   \emptyset "> , then  <img src="https://render.githubusercontent.com/render/math?math=P(A  \cup B) = P(A) %2b P(B)"> 

### Addition law of probability

The additivity axiom is great, but most of the time events are not exclusive. A very important property is the **addition law or probability** or the **sum rule**.

 <img src="https://render.githubusercontent.com/render/math?math=P(A  \cup B) = P(A) %2b P(B) - P(A    \cap B) "> 

Put in words, the probability that  <img src="https://render.githubusercontent.com/render/math?math=A"> or  <img src="https://render.githubusercontent.com/render/math?math=B"> will happen is the sum of the probabilities that  <img src="https://render.githubusercontent.com/render/math?math=A"> will happen and that  <img src="https://render.githubusercontent.com/render/math?math=B"> will happen, minus the probability that *both*  <img src="https://render.githubusercontent.com/render/math?math=A"> and  <img src="https://render.githubusercontent.com/render/math?math=B"> will happen.

## Examples

Let's reconsider the dice example to explain what was explained before:

### Additivity of exclusive events

Let's consider two events: event  <img src="https://render.githubusercontent.com/render/math?math=M"> means throwing a 6, event  <img src="https://render.githubusercontent.com/render/math?math=N"> means that you throw an odd number  <img src="https://render.githubusercontent.com/render/math?math=N={1,3,5}"> . These events are exclusive, and you can use the additivity rule if you want to know the answer to the question: 

*"what is the probability that your outcome will be a 6, or an odd number?"*

 <img src="https://render.githubusercontent.com/render/math?math=P(M  \cup N) = P(M) %2b P(N) =   \dfrac{1}{6}%2b \dfrac{3}{6}= \dfrac{4}{6} "> 

### Addition law of probability

Now, let's consider the same event  <img src="https://render.githubusercontent.com/render/math?math=N={1,3,5}"> and another event  <img src="https://render.githubusercontent.com/render/math?math=Q={4,5}"> . These events are *not* mutually exclusive, so if you want to know the probability that  <img src="https://render.githubusercontent.com/render/math?math=N"> or  <img src="https://render.githubusercontent.com/render/math?math=Q"> will happen, you need to use the addition law of probability.

Note that  <img src="https://render.githubusercontent.com/render/math?math=(N    \cap Q)"> is equal to getting an outcome of 5, as that is the "common" element in the respective event spaces of  <img src="https://render.githubusercontent.com/render/math?math=N"> and  <img src="https://render.githubusercontent.com/render/math?math=Q"> . This means that  <img src="https://render.githubusercontent.com/render/math?math=P(N    \cap Q) =   \dfrac{1}{6}"> 

 <img src="https://render.githubusercontent.com/render/math?math=P(N  \cup Q) = P(N) %2b P(Q) - P(N    \cap Q) =   \dfrac{3}{6} %2b   \dfrac{2}{6} -   \dfrac{1}{6} =   \dfrac{4}{6} "> 


## Final Note

In the previous examples, you noticed that for our dice example, it is easy to use these fairly straightforward probability formulas to calculate probabilities of certain outcomes. 

However, if you think about our text message example, things are less straightforward, e.g.:

*"What is the probability of sending less than 20 text messages in a day?"*

This is where the probability concepts introduced here fall short. The probability of throwing any number between 1 and 6 with a die is always exactly  <img src="https://render.githubusercontent.com/render/math?math= \dfrac{1}{6}"> ,  but we can't simply count our messages event space. In words, the probability of sending 20 messages is likely different than the probability of sending, say, 5 messages, and will be different for any number of messages sent. You'll learn about tools to solve problems like these later on.


## Summary

Well done! In this section, you learned how to use sets to get to probabilities. You learned about experiments, event spaces, and outcomes. Next, you learned about the law of relative frequency and how it can be used to calculate probabilities, along with the three probability axioms.
