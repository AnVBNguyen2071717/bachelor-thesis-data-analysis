# Thesis: An Affectively Rational Decision

## The Interplay of Happiness Alignment and Venture Quality in Predicting Investor Funding Intentions

**Author:** An V.B. Nguyen
**Institution:** Tilburg University
**Date:** June 30, 2025
---

### Project Overview

This repository contains the complete data analysis pipeline and associated data files for the bachelor's thesis, "An Affectively Rational Decision." The research investigates the impact of dyadic emotional alignment on investor funding intentions in an entrepreneurial pitch context.

The workflow is designed for full transparency and reproducibility, starting from two primary sources and culminating in a final, analysis-ready dataset and the statistical models used to test the hypotheses.

### File Descriptions

This repository contains four key files that represent the stages of the data analysis process:

1.  **`investor_survey_filtered.csv`**
    * **Description:** This is the primary survey data, filtered to include only the 56 pitches for which valid video data was available. It contains the dependent variable (`probinv` - Funding Intention) and all investor-rated control variables.

2.  **`happiness_data_with_harmonized_ids.csv`**
    * **Description:** This is the primary time-series data file. It is the result of consolidating data from two different facial expression analysis tools (OpenFace and FaceReader) and includes a crucial `session_id` column that has been programmatically cleaned and harmonized to match the `startup` names in the survey data.

3.  **`FINAL_ANALYSIS_DATASET_UNSTANDARDIZED.csv`**
    * **Description:** This is the final, analysis-ready dataset where each row represents one investor's evaluation of one pitch (a dyad). It contains the calculated predictor variables for all three hypotheses (e.g., `Duration_of_Aligned_Peak_Happiness`, `Consensus_of_Alignment`) and the control variables, all in their original, unstandardized units. This file is used to generate the descriptive statistics table.

4.  **`Thesis Analysis.ipynb`**
    * **Description:** This Jupyter Notebook contains the complete Python code pipeline used for this study. It details all steps, including:
        * Loading and harmonizing the source data.
        * Calculating the predictor variables for H1, H2, and H3.
        * Standardizing the variables for modeling.
        * Running the final multilevel regression models.
        * Generating all APA-7 style tables and figures presented in the thesis.

### Abstract

Securing funding is a critical hurdle for new ventures, and the entrepreneurial pitch is the primary arena where investors make their evaluations. While theory suggests that an entrepreneur's positive emotions can be "caught" by investors, this thesis tests the effect of this dyadic emotional alignment on funding decisions. Drawing on Emotional Contagion Theory and Event System Theory, this study uses frame-by-frame facial expression data from 56 real entrepreneurial pitches. The results from multilevel regression models show that while the duration of aligned happiness significantly predicts funding intention, the consensus and timing of this alignment do not. Furthermore, the analysis consistently and powerfully revealed that the investors' rational assessment of the venture's quality was the dominant predictor. This study contributes to the literature by establishing a clear boundary condition for the effects of emotional contagion in a professional, evaluative context, suggesting that while emotional dynamics are present, they are overridden by a deliberate focus on the substantive merits of the venture.
