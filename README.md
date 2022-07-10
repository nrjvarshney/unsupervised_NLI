# Unsupervised Natural Language Inference 

Public repository associated with [Unsupervised Natural Language Inference Using PHL Triplet Generation, ACL 2022](https://arxiv.org/abs/2110.08438).

# Abstract
Transformer-based models have achieved impressive performance on various Natural Language Inference (NLI) benchmarks when trained on respective training datasets.
However, in certain cases, training samples may not be available or collecting them could be time-consuming and resource-intensive.
In this work, we address the above challenge and present an explorative study on unsupervised NLI, a paradigm in which no human-annotated training samples are available.
We investigate it under three settings: _PH, P_, and _NPH_ that differ in the extent of unlabeled data available for learning.
As a solution, we propose a procedural data generation approach that leverages a set of sentence transformations to collect PHL (Premise, Hypothesis, Label) triplets for training NLI models, bypassing the need for human-annotated training data.
Comprehensive experiments show that this approach results in accuracies of _66.75%, 65.9%,  65.39%_ on SNLI in PH, P, and NPH settings respectively, outperforming all existing unsupervised baselines.
Furthermore, fine-tuning our model with as little as _~0.1%_ of the training dataset (_500_ instances) leads to _12.2%_ higher accuracy than the model trained from scratch on the same _500_ instances.
Supported by this superior performance, we conclude with a recommendation for collecting high-quality task-specific data.



<p align="center">
  <img 
    width="300"
    height="300"
    src="https://github.com/nrjvarshney/unsupervised_NLI/blob/main/Pictures/Teaser4.png"
  >
  <figcaption>Figure 1: Illustrating our procedural data generation approach for unsupervised NLI. A sentence is treated as premise, and multiple hypotheses conditioned on each label (Entailment- E, Contradiction- C, and Neutral- N) are generated using a set of sentence transformations. </figcaption>
</p> 


# NLI Data Generation Approaches

1. **Entailment** - Paraphrasing, Extracting Snippets, Hypernym Substitution, Pronoun Substitution, Counting
3. **Contradiction** - Contradictory Words, Contradictory Verbs, Subject Object Swap, Negation Introduction, Number Substitution, Irrelevant Hypothesis
4. **Neutral** - Adding Modifiers, ConceptNet, Same Object but Non-Contradictory Verb, Composite Methods


# Implementation
- Will be uploaded by 16 July 2022
