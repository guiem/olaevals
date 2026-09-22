# HUME[^1] (Human Understanding & Modeling Evaluation)

## Description

Anthropognostic Evaluations, aka "do AIs understand humans?", encompass a set of tests aimed at measuring the understanding of the human condition, and surfacing the gap between machines and humans on the matter.

The main thesis is that anthropognosis, a strong understanding of humans, is a safety-relevant capability whose absence, presence, and interaction with other capabilities should be measured ("AI that affects humans should understand humans"). Whether a higher degree of human understanding is a necessary condition for safer AI remains an open research question[^2]. It is, however, unlikely to be sufficient[^3]: a better understanding of humans may enable safer and more beneficial behavior, but it may also increase a system's capacity for manipulation, persuasion, deception, explotaition or coercion.

In the event of an Artificial Superintelligence[^4] (ASI), consequences can be catastrophic if such ASI does not understand humanity. A subset of this problem could be even the inability to communicate with humans.

This project is aimed at kickstarting a research agenda which main goals:
1. define what "understanding humans/humanity" mean[^5]
2. operationalize such construct[^6]
3. design an evaluation/s to measure anthropognosis[^7]
4. create a framework to interpret implications of different range of levels in anthropognosis.

If we can successfully assess anthropognostic capabilities, doing so could help reduce, or at least better understand, the risks posed by advanced AI systems. Knowing where and how AI systems misunderstand humans could inform deployment decisions, training, safeguards, and the interpretation of other evaluations. This may be especially important in high-stakes situations where communication and conflict resolution matter: if an advanced system can genuinely understand human intentions, values, concerns, and the consequences its actions have for people, then we at least have a stronger basis for meaningful and transparent communication with it. More immediately, measuring the extent to which AI systems understand humans could also provide useful context for interpreting their behavior in other safety evaluations.


## Risk Analysis
- “Communication is necessary for conflict resolution” is reasonable but may not be enough, understanding humans does not guarantee cooperative communication. Understanding capability may need to be combined with alignment/cooperation/corrigibility to provide actual safer interaction. 
- “AI has skin in the game and therefore won't sandbag”. A sufficiently strategic model could understand that passing or failing has downstream consequences. 
- Dynamnically generated tests introduce another problem: how do you guarantee equivalent difficulty and construct validity? Need to evaluate the evaluator. One big research question is whether we are capable to find a trivial mechanism which helps us with this generation. The research assumption is that a binary wall exists that has to be crossed in order to understand humans, at least the way we do. An analogy would be a child that is not capable of reading words yet, even though they are capable of reading phonems from letters, until the brain is ready the sequence of sounds does not form a word. 

## Project Expansion

This project is the stepping stone of a broader agenda, timeline and future projections:
1. Establish the research program (also gather empirical evidence for HUME: the first Anthropognostic evaluation). 3 months.
2. Create a Foundation. Grow distributed team (anywhere in the world so the field benefits from diversity). Consolidate first anthropognostic evaluation. 6 months.
3. Broaden scope from benchmark/eval creation to auditing existing evaluations (borrow current red teaming of models to red teaming existing evaluations)



[^1]: a little nod to David Hume, 1) empiricism: claims about AI understanding should be supported by observed behavior and empirical evidence, 2) human nature: how humans actually think, feel, judge, and behave, 3) epistemic humility: evaluations provide evidence, not certainity, conclusions should reflect the limits of what's tested.
[^2]: [gather scientific evidence if possible][
[^3]: find literature on psychopaths, and their ability of having a good mental model of others, and yet representing a threat to other humans]
[^4]: [assumes an intelligence way higher than any human being is unable to understand or not communicate with human beings. One could argue around the definition of ASI, making it a necessary condition to claim it is ASI, however, we base ourselves from the point of view of an analogy where human beings are not able to communicate or fully understand ants]
[^5]: What does it mean to be human? What's only human (sense of humor, compassion…)? Do humans even understand humans?
[^6]: Same way we can say "AI has solved Navier-Stokes", can we at least approximate "AI understands humans"?
[^7]: A desirable design implies that 1) tests should be dynamic, we should be able to generate endless tests similar to the endless generative power of grammar so we avoid contamination, 2) tests should be trivial to pass by humans, but hard for machines, 3) AI has some skin in the game, wants to pass the test since humans wouldn't allow it to do anything if it doesn't pass it, so AI naturally doesn't want to sandbag, and 4) passing the test/s would add to an AI's portfolio, it should be a requirement but not a sufficient condition for anything, e.g. for certain environments and model capabilities, they should pass the HUME eval.




