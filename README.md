# PHP 2550 PDA Project3: Optimizing Cluster-Randomized Trial Designs

## Summary
This project investigates the optimization of recruitment strategies for cluster-randomized trials under budget constraints. Through hierarchical modeling, we examine both normal and poisson distributions to understand how different outcome types affect trial design. The core focus lies in determining the optimal balance between the number of clusters (G) and observations per cluster (R), while operating within fixed budget constraints (B). Our analysis incorporates realistic cost considerations, including the expenses associated with recruiting new clusters (c1) and gathering additional measurements within existing clusters (c2). The study systematically varies key parameters – the intercept (α), treatment effect (β), and cluster-level variance (γ2) – to comprehensively understand their influence on design choices and estimation precision.

<div align="center">
  <img width="500" alt="gamma_plot" src="https://github.com/user-attachments/assets/f5c34a70-4c58-4bed-94b8-69f3465216aa" />
</div>

Our findings demonstrate that increasing the number of clusters (G) consistently enhances the precision of treatment effect estimates, as shown through reduced variance and mean squared standard errors. However, the optimal recruitment strategy adapts to economic realities: when the cost per cluster (c1) rises, the most efficient approach shifts toward establishing fewer clusters while collecting more observations within each one. This relationship becomes particularly evident when examining relative cost ratios (c1/c2), where higher ratios strongly favor increasing within-cluster observations over adding new clusters. The comparison between normal and poisson models reveals important distinctions in their behavior. The poisson model demonstrates notably higher sensitivity to parameter variations and exhibits greater variability, especially with smaller cluster sizes. This instability becomes more pronounced as cluster-level variance (γ2) increases. However, both models benefit from larger treatment effects (β), which strengthen the signal-to-noise ratio and improve overall estimate stability.

<div align="center">
  <img width="250" alt="gamma_tbl" src="https://github.com/user-attachments/assets/99eb7b3b-7d0e-4afa-889a-56f73e845089" />
</div>

Our research provides actionable insights for researchers designing cluster-randomized trials with budget constraints. These findings offer evidence-based guidance for resource allocation decisions while highlighting the importance of considering distributional assumptions in trial design. Future research directions could enhance these insights by incorporating more complex inter-cluster relationships, addressing missing data scenarios, and exploring the interactions between nested parameters.

## Folders and Files
`project3.qmd`: This file contains R code and text explanations for the Simulation Design and Results Analysis.

`project3.pdf`: A PDF version of the report, including the Code Appendix at the end.

Data: Simulated datasets stored in CSV files.

Perf: Performance measures stored in CSV files.

## Dependencies
I used the following packages for this analysis: knitr, dplyr, tidyr, ggplot2, gridExtra, grid, purrr, lme4,and  Rlab.
