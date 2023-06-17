---
title: "Poster - Screening peripheral biopsies for alpha-synuclein pathology using deep machine learning"
collection: talks
type: "Talk"
permalink: /talks/2020-07-28-peripheral-biopsies 
venue: "Alzheimer's Associated International Conference"
date: 2020-07-28
location: "Virtual Event"
---

[More information here](https://alz.confex.com/alz/20amsterdam/meetingapp.cgi/ModuleMeetingInfo/0)

Background: Post-mortem assessment remains the only option and a gold standard for a definitive diagnosis of Parkinson’s disease (PD). The antemortem diagnosis is challenging due to a variable clinical presentation and the abundance of mimicking conditions, obscuring the clinical picture and delaying the treatment. It is well established that while PD pathologically manifests in central nervous system with aggregation of α-synuclein as Lewy bodies and Lewy neurites, this pathology is also found in the peripheral nervous system. Peripheral Lewy-type synucleinopathy (LTS) is present in early PD, suggesting its utility as a diagnostic and prognostic biomarker. We have previously confirmed that detection of LTS in submandibular gland (SMG) biopsies is sensitive (.75) and specific (.90) for early PD. However, the assessment by a neuropathologist of multiple levels of such biopsy is laborious and time-consuming.

Method: Here work we applied two Convolutional Neural Networks (CNN) for detection of LTS on 283 digital whole slide images (WSI) from 95 unique SMG biopsies. A total number of 8,386 LTS were annotated following the interrater reliability study with kappa=.7. We used transfer learning to train a CNN model to classify image patches (40-by-40 pixels at 20x) with and without presence of LTS objects.

Result: The trained CNNs showed the following performance on image patches: sensitivity: .982/.988, specificity: .998/.999, precision: .852/.950, accuracy: .995/.998, and F-1 score .912/.968 for ResNet30/InceptionV4 respectively. On test WSI the sensitivity in detecting LTS was .963/.971 respectively.

Conclusion: This work is first to demonstrate the practical utility of an CNN for screening for LTS, which can further translate into a practical screening tool facilitating the antemortem diagnosis of PD. We further plan to develop neural networks for accurate and precise detection and quantification of LTS in antemortem SMG biopsies. This, altogether, would offer a screening, confirmatory, prognostic, and quantitative tool for clinical assessment of early PD.
