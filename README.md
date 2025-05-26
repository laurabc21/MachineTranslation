# COMET Evaluation Reliability Study on Catalan WMT2013 MT Test Set

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

## Methodology

1. We used the COMET model (`Unbabel/wmt22-comet-da`) to score all 3,000 translation segments.
2. A randomly selected subset of 140 segments was annotated by a human evaluator using a scoring scale aligned with COMET’s.
3. We then compared COMET scores with human scores using a ±0.2 threshold to identify:
   - **Equal**: Minor differences (within the threshold)
   - **Overestimation**: COMET scores significantly higher than human scores
   - **Underestimation**: COMET scores significantly lower than human scores
