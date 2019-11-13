+++
title = "Abstract"
widget = "blank"
headless = true
active = true
weight = 5

+++

## Unifying deep learning with item response theory: interval measurement, annotator debiasing, efficiency, and explainability

Outcomes are commonly measured as binary variables: a comment is toxic or not, an image has sexual content or it doesn’t, etc. But the real world is more complex: most target variables are inherently continuous in nature. Physical quantities such as temperature and weight can be measured as interval variables where magnitudes are meaningful. How can we achieve that same interval measurement for arbitrary outcomes - creating continuous scales with magnitudes?

We propose a method for measuring phenomena as continuous, interval variables by unifying deep learning with the *Constructing Measures* approach to Rasch item response theory (IRT). We decompose the target construct into ordinal components measured as survey items, which are then transformed via an IRT non-linear activation into a continuous measure of unprecedented quality. We estimate first-order labeler bias and eliminate its influence on the final construct when creating a training dataset, which supersedes the notion of inter-rater reliability as a quality metric. To our knowledge this IRT bias adjustment has never before been implemented in machine learning but is critical for algorithmic fairness. We further estimate the response quality of each individual labeler, allowing responses from low-quality labelers to be removed.

Our IRT scaling translates naturally into multi-task, weight-sharing deep learning architectures in which our theorized outcome components become supervised, ordinal latent variables for the neural networks’ internal representation learning. Our multitask architecture exploits a proportional odds activation function and quadratic weighted kappa loss function designed for ordinal outcomes. This leads to a new form of model explanation because each continuous prediction can be directly explained by the constituent ordinal components in the penultimate layer.

We demonstrate our method on a new dataset of 50,000 online comments labeled to measure a spectrum from hate speech to counterspeech, and sourced from YouTube, Twitter, and Reddit. We evaluate Universal Sentence Encoders, BERT, RoBERTa, and XLNet as contextual representation models for the comment text, and benchmark our predictive accuracy against Google Jigsaw’s Perspective API models.
