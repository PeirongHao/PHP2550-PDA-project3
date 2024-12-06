# PHP 2550 PDA project3

## Abstract
This simulation project investigates optimal recruitment designs for cluster-randomized trials within budgetary limitations. The project examines two data-generating models: normally distributed outcomes and poisson-distributed outcomes. Hierarchical data are generated with multiple parameters, such as the number of clusters ($G$), the number of observations per cluster ($R$), and cluster-level variance ($\gamma^2$). The simulation attempts to determine an optimal balance between $G$ and $R$ to reduce estimation variability. The comparative costs of sampling new clusters ($c_1$) versus conducting additional measurements within existing clusters ($c_2$) are adjusted to assess their influence on estimates. Models are fitted using linear mixed-effects models for the normal scenario and generalized linear mixed-effects models for the poisson scenario, with performance assessed through metrics including the variance of estimates and average of estimates' standard errors. Results indicate that increasing the number of clusters ($G$) improves precision within specified budgets. Higher budgets enable the inclusion of more clusters in both models; however, the normal model emphasizes increasing $R$, while the Poisson model prioritizes $G$. Larger $\beta$ values enhance estimate stability, while higher $\gamma^2$ amplifies variability, particularly in the Poisson model. As $C_1$ (cost per new cluster) increases, $G$ decreases, and higher relative cost ratios ($C_1/C_2$) make collecting additional observations within existing clusters more economical. Overall, the normal model exhibits greater stability than the Poisson model. These findings provide practical guidance for researchers designing cost-effective cluster-randomized trials.

## Folders and Files
project3.qmd: This file includes R code and text explanations for both the Exploratory Data Analysis and Statistical Analysis.
project3.pdf: A PDF version of the report, including a Code Appendix at the end.
Data: Simulated datasets stored in CSV files.
Performance: Performance measures include the estimated beta values and their corresponding standard errors.

## Dependencies
I used the following packages for this analysis: knitr, dplyr, tidyr, ggplot2, gridExtra, grid, purrr, lme4,and  Rlab.
