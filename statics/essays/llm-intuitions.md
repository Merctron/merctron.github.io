# LLM Intuitions

This is an attempt to re-cast what I've learned about language models (in particular, to do with transformers). In large part, I owe my understanding (as well as large chunks of this material) to the series of lectures by Andrej Karpathy, in particular this lecture on building a GPT from scratch. I hope to add maybe a simpler example and more detailed commentary at every step - the idea being that future me (or anyone else who finds this useful) can recover the full inituition for language models by just reading this.

## An Aside To Kick Things Off

I'm paraphrasing here from [the bitter lesson by Richard Sutton](http://www.incompleteideas.net/IncIdeas/BitterLesson.html). Every time humans have tried to model their own intelligence to build AI, they have failed. We tried to build logic driven inference systems to try and get the full understanding of domains to into thinking machines and that led to the first AI winter.

What does work, is simple mechanisms that can build upon themselves to emerge with something complex - basics like search, and re-enforcement (which I guess is just giving a machine the freedom to perform search within the bounds of some problem space). Finally, the simple mechanisms have to be paired with advances in compute to get the truly great results.


So far, this thesis seems to be holding true - large language models (LLMs) are performing very well with a simple idea (attention/self-attention) with a ton of compute resources thrown at them. I have not made up my mind about whether this paradigm will continue to pay dividends or whether some extra symbolic component will be needed to build something even more general and resilient to approach the abilities of a human brain - but the possibility cannot be ruled out (or at least it is not within my ability to theorize either way).

## What Are The Simple Mechanisms?

I will cast the complications of an LLM in the simplest terms as we go step by step to build one. We will journey across the following concepts from scratch.

Perceptrons -> Deep Neural Networks -> Bi-gram Language Models -> The mathematics of Attention -> Attention + Bi-gram models A.K.A Transformers 