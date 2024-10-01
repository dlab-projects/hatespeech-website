---
title: "Constructing interval variables via faceted Rasch measurement and multitask deep learning: a hate speech application"
authors:
- chris-kennedy
- geoff-bacon
- alexander-sahn
- claudia-von-vacano
date: "2024-01-07T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-09-22T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "Constructing interval variables via faceted Rasch measurement and multitask deep learning: a hate speech application"
# publication_short: ""
abstract: "We propose a general method for measuring complex variables on a continuous, interval spectrum by combining supervised deep learning with the Constructing Measures approach to faceted Rasch item response theory (IRT). We decompose the target construct, hate speech in our case, into multiple constituent components that are labeled as ordinal survey items. Those survey responses are transformed via IRT into a debiased, continuous outcome measure. Our method estimates the survey interpretation bias of the human labelers and eliminates that influence on the generated continuous measure. We further estimate the response quality of each labeler using faceted IRT, allowing responses from low-quality labelers to be removed.
Our faceted Rasch scaling procedure integrates naturally with a multitask deep learning architecture for automated prediction on new data. The ratings on the theorized components of the target outcome are used as supervised, ordinal variables for the neural networks' internal concept learning. We test the use of an activation function (ordinal softmax) and loss function (ordinal cross-entropy) designed to exploit the structure of ordinal outcome variables. Our multitask architecture leads to a new form of model interpretation because each continuous prediction can be directly explained by the constituent components in the penultimate layer.
We demonstrate this new method on a dataset of 50,000 social media comments sourced from YouTube, Twitter, and Reddit and labeled by 11,000 U.S.-based Amazon Mechanical Turk workers to measure a continuous spectrum from hate speech to counterspeech. We evaluate Universal Sentence Encoders, BERT, and RoBERTa as language representation models for the comment text, and compare our predictive accuracy to Google Jigsaw's Perspective API models, showing significant improvement over this standard benchmark."

# Summary. An optional shortened abstract.
# summary: ""

tags:
- Source Themes
featured: false

links:
#- name: Custom Link
#  url: https://dl.acm.org/doi/abs/10.1145/3531146.3533216
url_pdf: https://arxiv.org/abs/2009.10277
url_code: 'https://github.com/dlab-projects/hate_measure'
url_dataset: 'https://huggingface.co/datasets/ucberkeley-dlab/measuring-hate-speech'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ""
  focal_point: "center"
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
