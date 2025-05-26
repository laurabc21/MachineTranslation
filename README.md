# COMET Evaluation on Catalan 
## Overview

This project investigates the reliability of the COMET evaluation metric when applied to a machine translation dataset. Specifically, we infer COMET scores on the **Catalan WMT2013 Machine Translation Shared Task Test Set**, which contains **3,000 translation segments**. Our goal is to assess whether COMET scores align closely with human judgments, thereby validating its effectiveness for Catalan-English translation evaluation.

## Objectives

- To automatically evaluate translation quality using the **COMET** metric.
- To compare COMET scores with **human-annotated scores** on a subset of 140 segments.
- To analyze whether COMET can reliably approximate human judgments for Catalan machine translation.

## Dataset

- **Corpus**: WMT13 Machine Translation Shared Task - Catalan Test Set (https://elrc-share.eu/repository/browse/catalan-wmt2013-machine-translation-shared-task-test-set/84a96139b98611ec9c1a00155d0267061a0aa1b62e2248e89aab4952f3c230fc/)
- **Size**: 3,000 segments
- **Subset for human annotation**: 140 segments manually scored by a human annotator

## Codes in the folder

**API_Gemini.ipynb**
This notebook contains the code used to generate automatic translation outputs using the Gemini translation system.

**Comet_WholeDataset_Gemini.ipynb**
Computes COMET scores for all 3,000 segments in the dataset based on the Gemini translations.

**Distribution_Human_COMET.ipynb**
Compares the distribution of COMET scores and human annotations. Includes visualizations for qualitative analysis.

**Normalization_Fluency_Accuracy.ipynb**
Performs normalization of human evaluation scores (fluency and accuracy) to make them compatible with COMET's scoring range, enabling direct comparison.

