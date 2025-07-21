# Hacking Humans For Fun and Profit

As a freshman to a computer science program you quickly discover some lore - part of this was reading popular white papers when you get a few semesters deep into systems programming - one of these was [Smashing the Stack for Fun and Profit](https://inst.eecs.berkeley.edu//~cs161/fa08/papers/stack_smashing.pdf). Years later, artifacts that borrow the naming convention continue to appear and I thought I might join in having recently read the book [Alchemy](https://www.goodreads.com/book/show/26210508-alchemy). I think the name fits - much like stack smashing, this is a discussion about exploiting bugs in the human condition using psychologic.

## Primer On Human Bugs

There is now a healthy eco-system of books that seek to explain why economics is hog-wash and human decision-making is hard to model. Psychologists [Amos Tversky](https://en.wikipedia.org/wiki/Amos_Tversky), and [Daniel Kahneman](https://en.wikipedia.org/wiki/Daniel_Kahneman) began this work decades ago and it has (rightly) spread and been discussed in different contexts. Perhaps it is worth listing out what I have absorbed about this through what I've read, watched, or listened to.

First, the conceptual basis - System 1 and System 2 thinking:
* System 1 is fast twitch thinking. Our frontline agent. It relies on heuristics, stereotypes, and other frowned upon short cuts but it serves us well and is effortless to use.
* System 2 is slow, methodical, analytical. It's the part of the brain that hurts when you have to think really hard.

I should note, these don't exactly map neuro-anatomically (as far as I know) but our brain is likely wired up in a way to support this model - minor introspection into how I myself think leads me to believe this distinction holds up. In fact, this model also shows promise when it comes to [architecting autonomous agents using large langugage models](https://arxiv.org/pdf/2410.08328).

Our heuristic based System 1 is what we need to hack because that's where the bugs lie. We use it most often and System 2 is mostly engaged only to do System 1's bidding. Some of these bugs include:

* Self Deception and Hidden Motives - Claiming one thing and wanting another.
* The effectiveness of Placebos - System 1 is somehow tied in with activation of the immune system (or some other mysterious physiological mechanism) and being in the right circumstances to heal is not enough. You also need to believe that a cure is working its way through you.
* Loss Aversion - We are more likely to work to avoid a loss than to secure a gain. This may not be a bug but a feature since it leads to anti-fragility in the real world (ensemble expected values mean nothing if a misstep in a sequence of actions leads to death).
* Framing - How we deal with a choice depends on its packaging.
* Anchoring and Availability - We are senstive to information to a fault and will latch on to the first thing we focus on and make future decisions on that basis.
* The infamous sunk cost fallacy.
* Substitution effects - It's difficult to objectively analyze who the best person to elect president is based on their policy positions but it's easy to decide who to have beer with based on their vibe (and substitute the answer to the first question with the answer from the second).

## White Hat Human Hacking

[Alchemy](https://www.goodreads.com/book/show/26210508-alchemy) deals with human bugs by casting them as a higher-order magic that should be used (and indeed some of these bugs are features and exist for good reason).

Ordinarily, I would take some exception with blanket approval of what the author likes to call 'benign bullshit' but the book aquits itself in the following passage:

> But what about snake-oil salesmen, the fakers, fraudsters and conmen? Alchemy, precisely because it is not an exact science, has always been rife with charlatanry, and we should be on our guard for this. Many of the remedies proposed by people in advertising and design are wrong, and many of the findings of behavioural scientists have already been or will be proved wrong. Some parts of this book are also undoubtedly wrong – I am conscious that I have written this book from an incredibly optimistic perspective, but my argument is not that alchemy is always reliable, ethical or beneficial. Far from it – it is simply that we should not recoil from testing alchemical solutions because they do not fit with our reductionist ideas about how the world works. The purpose of this book is to persuade the reader that alchemy exists whether we like it or not, and that it is possible besides, if people are more aware of its existence, they will be better at spotting its misuses.

I don't think I need to add anything further than to say I agree with this take. Let's try to be aware of Human Bugs and exploit them so that everyone is better off (easier said than done).

## A CAP Theorem For Humans?

There's a [CAP theorem](https://en.wikipedia.org/wiki/CAP_theorem) for distributed systems - simply, among a choice of three desired properties, we can pick only two, and one of the more interesting insights from reading human decision making literature is that something similar exists in this less mathematically pure and more difficult to model realm. Rory Sutherland names one of his book's chapters to this effect:

> Efficiency, Logic, and Meaning - Pick Any Two

The problem I suppose, boils down to the transmission of information. Signalling trust for humans cannot be cheap because it needs to encode emotion, ethics, and culture and pursuing utility theory based efficiences seems to sacrifice the expensive meaning that needs to be signalled at the alter of logic and efficiency. The properties being selected are not a good fit for a species that are built to bias toward System 1 thinking.

Some of these are semantic games as well. Ruthless, sterile corporate efficiency is not really efficient when applied to a system where it does not work and produces terrible effects in the long term. In the book [Beyond Self-Interest](https://www.goodreads.com/book/show/58986900-beyond-self-interest), Krzysztof Pelc argues that the market actually rewards those that start businesses to pursue a passion or solve a problem as its own end with profit being, at best, a secondary motivation - I can't help but think that this a restatement of the alchemical hacking of human brains, or expensive signalling that demonstrates skin in the game, or antifragility being an attractive quality in human endeavours. The more complex and networked a system is, the more information needs to be transmitted with a high quality signal to ensure trust.

Focusing back on the CAP theorem, if we want to transmit meaning while being efficient, we must give up logic. This is not because there is not some rational explanation in play, but rather because the explanation is so complex that it cannot be discovered by the current methods of logic and reason. Rather, we must stumble upon efficient and meaning rich transimission mechanisms by experimentation.

## Coordination Problems

So far the discussion of Human Bugs, decision making, and information transmission has leaned toward persuasion as the ends. However, one of the things we end up spending a lot of our time on is coordination. My experience is primarily driven by the corporate cultures I have worked in so far - teams and heirarchies of smart and well meaning people who are trying to navigate incentives to grow their own career while doing right by customers, their colleagues, and even the business they work for. Even the most well run organizations, run into these issues at scale, and even here it seems [that properties of complex adaptive systems are at play](https://surfingcomplexity.blog/2025/06/08/ai-at-amazon-a-case-study-of-brittleness/). I have a feeling there is a non-intuitive answer for how to solve this (one that will fly in the face of most managerial wisdom) but this needs more thinking through. Alternatively, someone smarter than me will come up with an answer and I'll just document the insight here.

## What To Write About Next?

* Status games
* Adapting methods to the type of Human
  - Benefits of and different types of second brains

