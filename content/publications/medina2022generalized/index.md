---
title: Generalized property-based encoders and digital signal processing facilitate predictive tasks in protein engineering
authors:
- David Medina-Ortiz
- me
- Juan Amado-Hinojosa
- Jorge Torres-Almonacid
- Juan A. Asenjo
- Marcelo Navarrete
- Alvaro Olivera-Nappa
author_notes:
- ''
- Corresponding Author
- ''
- ''
- ''
- ''
- Corresponding Author
date: '2022-07-01'
publishDate: '2022-07-01'
publication_types:
- article-journal
publication:
  name: Frontiers in Molecular Bioscience
  volume: '9'
  pages: '898627'
peer_reviewed: true
abstract: Computational methods in protein engineering often require encoding amino acid sequences, i.e., converting them into numeric arrays. Physicochemical properties are a typical choice to define encoders, where we replace each amino acid by its value for a given property. However, what property (or group thereof) is best for a given predictive task remains an open problem. In this work, we generalize property-based encoding strategies to maximize the performance of predictive models in protein engineering. First, combining text mining and unsupervised learning, we partitioned the AAIndex database into eight semantically-consistent groups of properties. We then applied a non-linear PCA within each group to define a single encoder to represent it. Then, in several case studies, we assess the performance of predictive models for protein and peptide function, folding, and biological activity, trained using the proposed encoders and classical methods (One Hot Encoder and TAPE embeddings).
  Models trained on datasets encoded with our encoders and converted to signals through the Fast Fourier Transform (FFT) increased their precision and reduced their overfitting substantially, outperforming classical approaches in most cases. Finally, we propose a preliminary methodology to create de novo sequences with desired properties. All these results offer simple ways to increase the performance of general and complex predictive tasks in protein engineering without increasing their complexity.
summary: Computational methods in protein engineering often require encoding amino acid sequences, i.e., converting them into numeric arrays. Physicochemical properties are a typical choice to define…
featured: false
tags: []
hugoblox:
  ids:
    doi: 10.3389/fmolb.2022.898627
links:
- type: pdf
  url: https://www.frontiersin.org/articles/10.3389/fmolb.2022.898627/full
image:
  caption: 'Image credit: The Authors'
  focal_point: ''
  preview_only: false
---
