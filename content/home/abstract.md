+++
title = "Abstract"
widget = "blank"
headless = true
active = true
weight = 5

+++

## Measuring hate speech by integrating ordinal, multitask deep learning with faceted Rasch modeling

Outcome phenomena are typically measured at the binary level: a comment is toxic or not, an MRI scan shows cancer or is clear, a patient is diagnosed as having a disease or not. But underlying that dichotomization there is often a continuous spectrum or latent variable. Physical quantities such as temperature and weight can be measured as interval variables where magnitudes are meaningful. How can we achieve that same interval measurement for arbitrary outcomes - creating continuous scales with magnitudes?

We propose a general method for measuring complex phenomena as continuous, interval variables by integrating deep learning with the *Constructing Measures* approach to faceted Rasch item response theory (IRT).
We decompose the target construct into multiple constituent components that are labeled as ordinal survey items, and are transformed via an IRT nonlinear activation into a high-quality continuous measure. We estimate the survey interpretation bias of the human labelers and eliminate its influence on the final construct when creating a training dataset, which removes labeling bias and supersedes the use of inter-rater reliability as a quality diagnostic. We further estimate the response quality of each individual labeler using faceted IRT, allowing responses from low-quality labelers to be removed.

Our faceted Rasch scaling procedure corresponds naturally to a multitask, weight-sharing deep learning architecture in which our theorized components of the target outcome are used as supervised, ordinal latent variables for the neural networks' internal concept learning, improving sample efficiency and promoting generalizability. The architecture combines a proportional odds activation function and quadratic weighted kappa loss function designed for ordinal outcomes. This leads to a new form of model explanation because each continuous prediction can be directly explained by the constituent ordinal components in the penultimate layer.

We demonstrate our method on a new dataset of 50,000 social media comments labeled to measure a spectrum from hate speech to counterspeech, and sourced from YouTube, Twitter, and Reddit. We evaluated Universal Sentence Encoders, BERT, RoBERTa, ALBERT, and T5 as contextual representation models for the comment text, and benchmarked our predictive accuracy against Google Jigsaw's Perspective API models.
