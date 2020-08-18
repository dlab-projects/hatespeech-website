+++
title = "Abstract"
widget = "blank"
headless = true
active = true
weight = 5

+++

## Constructing interval variables via faceted Rasch measurement and multitask deep learning: a hate speech application 

We propose a general method for measuring complex variables on a continuous, interval spectrum by combining supervised deep learning with the *Constructing Measures* approach to faceted Rasch item response theory (IRT).
We decompose the target construct, hate speech in our case, into multiple constituent components that are labeled as ordinal survey items.
Those survey responses are transformed via an IRT nonlinear activation into a debiased, continuous outcome measure.
Our method estimates the survey interpretation bias of the human labelers and eliminates that influence on the generated continuous measure; removing labeling bias supersedes the use of inter-rater reliability as a quality diagnostic. We further estimate the response quality of each individual labeler using faceted IRT, allowing responses from low-quality labelers to be removed.

Our faceted Rasch scaling procedure integrates naturally with a multitask, weight-sharing deep learning architecture for automated prediction on new data.
The ratings on the theorized components of the target outcome are used as supervised, ordinal latent variables for the neural networks’ internal concept learning, improving sample efficiency and promoting generalizability.
We test the use of a neural activation function (ordinal softmax) and loss function (ordinal cross-entropy) designed to exploit the structure of ordinal outcome variables.
Our multitask architecture leads to a new form of model interpretation because each continuous prediction can be directly explained by the constituent ordinal components in the penultimate layer.

We demonstrate this new method on a dataset of 50,000 social media comments sourced from YouTube, Twitter, and Reddit and labeled by 10,000 United States-based crowdsource workers to measure a continuous spectrum from hate speech to counterspeech.
We evaluate Universal Sentence Encoders, BERT, ELECTRA, and RoBERTa as language representation models for the comment text, and compare our predictive accuracy to Google Jigsaw’s Perspective API models, showing significant improvement over this standard benchmark.
