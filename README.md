This repository contains scripts for the data preprocessing and analysis for "Neural and behavioral reward responsiveness in early adolescence: longitudinal associations with childhood adversity and resilience", which used the ABCD 5.1 release.


The repository includes 7 scripts used for the primary analyses, which should be run sequentially:

"1_data_preprocessing" is adapted from a script provided by Brieant et al (2023), and details the pre-processing steps for the item-level adversity data.

"2_MICE" details the multiple imputation by chained equations procedure carried out using the item-level adversity data to account for missingness.

"3_get_adversity_factor_scores" details the factor score calculation procedure using 10 imputed item-level datasets, and the factor loadings matrix provided by Brieant et al. (2023) (included in "Adversity_factor_loadings").

"4_clean_MRI_data" details the exclusion of Monetary Inventive Delay data based on ABCD's quality control pipeline, which flags data based on behavioural task performance and poor image quality.

"5_create_datasets_for_mlm" details the cleaning and merging of covariate and outcome data to create analysis datatsets for the mixed effects models.

"6_mlm_models" details the implementation of the mixed effects/multilevel models, using the cleaned neural and behavioural datasets.

"7_plots" includes the scripts used for data visualisation. The plot outputs from this script were then finalised for publication using Inkscape.


We also include additional scripts for the supplementary analyses carried out ("Supplementary_analysis" folder), and the scripts for testing and visualising each of the age- sex- and resilience- related interactions ("Interactions" folder) using multivariate Wald tests and emtrends to compute linear combination of beta coefficients.





References:

Brieant A, Vannucci A, Nakua H, Harris J, Lovell J, Brundavanam D et al. Characterizing the dimensional structure of early-life adversity in the Adolescent Brain Cognitive Development (ABCD) Study. Dev Cogn Neurosci 2023; 61: 101256.
