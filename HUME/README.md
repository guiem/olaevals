# HUME[^1] (Human Understanding & Modeling Evaluation)

## Description

Anthropognostic evaluations—“do AIs understand humans?”—are tests aimed at measuring aspects of an AI system’s understanding of humans and identifying systematic gaps between machine and human performance. *Anthropognosis* is used here as a working umbrella construct, not as the assumption that human understanding is a single ability or can be captured by one score.

The main thesis is that anthropognosis is a safety-relevant capability whose absence, presence, and interaction with other capabilities should be measured (“AI that affects humans should understand humans”). Whether a higher degree of human understanding is a necessary condition for safer AI remains an open research question[^2]. It is unlikely to be sufficient[^3]: better models of humans may enable safer and more beneficial behavior, but may also increase a system’s capacity for manipulation, persuasion, deception, exploitation, or coercion.

Existing research provides a useful starting point but not a complete measure of anthropognosis. For example, theory of mind—the ability to represent other people’s mental states—is itself a family of related abilities rather than a unitary construct. Recent experiments have found that large language models can match or exceed human performance on some theory-of-mind tasks while failing others; they also show that apparent successes and failures can reflect response biases rather than the underlying capacity of interest.[^5] HUME therefore proposes a broader, construct-valid evaluation program rather than another isolated benchmark.

The longer-term motivation concerns advanced AI, including hypothetical artificial superintelligence (ASI). A highly capable system that systematically misunderstands human intentions, values, vulnerability, or the consequences of its actions could create serious risks. This is a motivating hypothesis, not an established empirical claim.[^4]

This project aims to begin a research agenda with four goals:

1. Define the dimensions of “understanding humans” that may be safety-relevant.[^5]
2. Operationalize those dimensions as measurable constructs.[^6]
3. Design evaluations that measure them validly and reliably.[^7]
4. Develop a framework for interpreting what different performance profiles do—and do not—imply.

If anthropognostic capabilities can be assessed successfully, the resulting evidence could help identify and characterize risks from advanced AI systems. Knowing where and how systems misunderstand humans could inform deployment decisions, training, safeguards, and the interpretation of other safety evaluations. It may also inform future assurance or regulatory evaluation practices, although current regulation does not specifically require an anthropognostic evaluation.[^8]

This may be especially relevant in high-stakes situations where communication and conflict resolution matter. Understanding human intentions and concerns could support more meaningful communication, but only when combined with properties such as cooperation, corrigibility, and appropriate objectives. More immediately, anthropognostic measurements could provide useful context for interpreting behavior in other safety evaluations.

## Risk Analysis

- **Construct breadth:** “Understanding humans” may be too broad to treat as one construct. It may include beliefs and intentions, emotions, social norms, values, culture, moral judgment, communication, vulnerability, humor, and conflict. HUME should first decompose anthropognosis into dimensions, then test which dimensions predict which safety-relevant behaviors.
- **Construct validity:** A test can be reliable while measuring the wrong thing. Each proposed measure needs an explicit construct definition, evidence that items elicit the intended capability, and tests of plausible alternative explanations.[^6]
- **Capability is not disposition:** Understanding another person does not imply caring about them. Research distinguishing cognitive from affective empathy provides a human analogy for why social modeling and prosocial motivation should not be conflated.[^3]
- **Human comparison:** Tasks need well-characterized human baselines and disagreement, not an assumption that every important item is trivial for every human. Comparisons should use multiple tasks, repetitions, and perturbations rather than one prompt or aggregate score.[^5]
- **Contamination and dynamic testing:** Generating or refreshing items may reduce contamination, but it can also change difficulty and construct coverage. Item generation therefore needs its own validation and quality controls.[^7]
- **Strategic behavior:** Giving a system “skin in the game” does not guarantee truthful performance. A sufficiently strategic system may infer the consequences of passing or failing, so sandbagging remains a threat model rather than a solved design problem.
- **Threshold assumptions:** The idea that human understanding requires crossing a binary threshold is an empirical hypothesis. HUME should compare threshold, continuous, and multidimensional models rather than assume one in advance.

## Project Expansion

This project is a stepping stone toward a broader agenda:

1. Establish the research program and gather initial empirical evidence through the first HUME evaluation. Target: 3 months.
2. Create a foundation, grow a distributed team, and consolidate the first anthropognostic evaluation. Target: 6 months.
3. Broaden the scope from creating evaluations to auditing them: apply adversarial and red-team methods not only to models, but to the evaluations used to make claims about them.

[^1]: A nod to David Hume: (1) **empiricism**—claims about AI understanding should be supported by observed behavior and empirical evidence; (2) **human nature**—the object of study is how humans actually think, feel, judge, and behave; and (3) **epistemic humility**—evaluations provide bounded evidence, not certainty.

[^2]: No cited result currently establishes anthropognosis as a necessary condition for safe AI. The necessity claim is treated as a falsifiable research question. Existing work instead supports studying narrower components and their limits; see [Strachan et al. (2024), “Testing theory of mind in large language models and humans,” *Nature Human Behaviour*](https://doi.org/10.1038/s41562-024-01882-z).

[^3]: Human evidence supports separating the capacity to infer another person’s mental state from affective concern for them; see [Campos, Rocha, and Barbosa (2023), “Dissociating cognitive and affective empathy across psychopathy dimensions,” *Frontiers in Psychology*](https://doi.org/10.3389/fpsyg.2023.1082965). This is an analogy, not evidence that AI systems have psychopathy. On the AI side, recent experiments show that language models can be effective persuaders, illustrating the dual-use potential of modeling an interlocutor; see [Salvi et al. (2025), “On the conversational persuasiveness of GPT-4,” *Nature Human Behaviour*](https://doi.org/10.1038/s41562-025-02194-6).

[^4]: ASI is used here as a hypothetical system substantially more capable than humans across many relevant domains. Claims about how such a system would understand or communicate with humans are currently speculative and should not be presented as empirical findings.

[^5]: Theory of mind offers one scientifically developed—but incomplete—starting point. Strachan et al. describe it as an interconnected set of abilities and compare humans and language models across false belief, indirect requests, irony, misdirection, and faux pas using repeated tests and novel items: [Strachan et al. (2024)](https://doi.org/10.1038/s41562-024-01882-z).

[^6]: Operationalization should be treated as a validation program, not merely the act of writing test items. See [Flake and Fried (2020), “Measurement Schmeasurement: Questionable Measurement Practices and How to Avoid Them,” *Advances in Methods and Practices in Psychological Science*](https://doi.org/10.1177/2515245920952393), and [Flake et al. (2022), “Construct validity and the validity of replication studies,” *American Psychologist*](https://doi.org/10.1037/amp0001006).

[^7]: A desirable design would use multiple measures, repeated trials, adversarial perturbations, human baselines, and novel or refreshed items. Dynamic items can reduce exposure to test-set contamination, but require stable scoring and difficulty controls. See [Strachan et al. (2024)](https://doi.org/10.1038/s41562-024-01882-z) and [White et al. (2024), “LiveBench: A Challenging, Contamination-Limited LLM Benchmark”](https://arxiv.org/abs/2406.19314).

[^8]: The [EU AI Act, Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) requires risk management and appropriate levels of accuracy, robustness, and cybersecurity for high-risk AI systems (notably Articles 9 and 15). It does not currently mandate a general evaluation of whether AI systems “understand humans.”
