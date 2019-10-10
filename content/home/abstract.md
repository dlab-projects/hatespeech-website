+++
title = "Abstract"
widget = "blank"
headless = true
active = true
weight = 5

+++

## Unifying deep learning with item response theory: interval measurement, annotator debiasing, efficiency, and explainability

Outcome phenomena are typically measured at the binary level: a comment is toxic or not, an image has sexual content or it doesn't, a patient is healthy or deceased. But the real world is more complex: most target variables are inherently continuous in nature. Physical quantities such as temperature and weight can be measured as interval variables where magnitudes are meaningful. How can we achieve that same interval measurement for arbitrary outcomes - creating continuous scales with magnitudes?

We propose a method for measuring phenomena as continuous, interval variables by 
unifying deep learning with the *Constructing Measures* approach to Rasch item response theory (IRT). 
The crux of our method is decomposing the target construct into multiple constituent components measured as ordinal survey items, which are then transformed via an IRT non-linear activation into a continuous measure of unprecedented quality. In particular, we estimate first-order labeler bias and eliminate its influence on the final construct when creating a training dataset, which renders obsolete the notion of inter-rater reliability as a quality metric. To our knowledge this IRT bias adjustment has never before been implemented in machine learning but is critical for algorithmic fairness. We further estimate the response quality of each individual labeler, allowing responses from low-quality labelers to be removed.

Our IRT scaling procedure fits naturally into multi-task, weight-sharing deep learning architectures in which our theorized components of the target outcome are used as supervised, ordinal latent variables for the neural networks' internal representation learning, improving sample efficiency and promoting generalizability. Built-in explainability is an inherent advantage of our method, because the final numeric prediction can be directly explained by the predictions on the constituent components.

We demonstrate our method on a new dataset of 50,000 online comments labeled to measure a spectrum from hate speech to counterspeech, and sourced from YouTube, Twitter, and Reddit. We evaluate Universal Sentence Encoders, RoBERTa, and XLNet as contextual representation models for the comment text, and benchmark our predictive accuracy against Google Jigsaw's Perspective API models.
