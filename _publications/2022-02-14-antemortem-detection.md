---
title: "Antemortem detection of Parkinson’s disease pathology in peripheral biopsies using artificial intelligence"
collection: publications
permalink: /publication/2022-02-14-antemortem-detection
excerpt: 'The diagnosis of Parkinson’s disease (PD) is challenging at all stages due to variable symptomatology, comorbidities, and mimicking conditions. Postmortem assessment remains the gold standard for a definitive diagnosis. While it is well recognized that PD manifests pathologically in the central nervous system with aggregation of α-synuclein as Lewy bodies and neurites, similar Lewy-type synucleinopathy (LTS) is additionally found in the peripheral nervous system that may be useful as an antemortem biomarker. We have previously found that detection of LTS in submandibular gland (SMG) biopsies is sensitive and specific for advanced PD; however, the sensitivity is suboptimal especially for early-stage disease. Further, visual microscopic assessment of biopsies by a neuropathologist to identify LTS is impractical for large-scale adoption. Here, we trained and validated a convolutional neural network (CNN) for detection of LTS on 283 digital whole slide images (WSI) from 95 unique SMG biopsies. A total of 8,450 LTS and 35,066 background objects were annotated following an inter-rater reliability study with Fleiss Kappa = 0.72. We used transfer learning to train a CNN model to classify image patches (151 × 151 pixels at 20× magnification) with and without the presence of LTS objects. The trained CNN model showed the following performance on image patches: sensitivity: 0.99, specificity: 0.99, precision: 0.81, accuracy: 0.99, and F-1 score: 0.89. We further tested the trained network on 1230 naïve WSI from the same cohort of research subjects comprising 42 PD patients and 14 controls. Logistic regression models trained on features engineered from the CNN predictions on the WSI resulted in sensitivity: 0.71, specificity: 0.65, precision: 0.86, accuracy: 0.69, and F-1 score: 0.76 in predicting clinical PD status, and 0.64 accuracy in predicting PD stage, outperforming expert neuropathologist LTS density scoring in terms of sensitivity but not specificity. These findings demonstrate the practical utility of a CNN detector in screening for LTS, which can translate into a computational tool to facilitate the antemortem tissue-based diagnosis of PD in clinical settings.'
date: 2022-02-14
venue: 'Acta Neuropathologica Communications'
paperurl: 'https://doi.org/10.1186/s40478-022-01318-7'
citation: 'Signaevsky, M., Marami, B., Prastawa, M. et al. Antemortem detection of Parkinson’s disease pathology in peripheral biopsies using artificial intelligence. acta neuropathol commun 10, 21 (2022).'
---