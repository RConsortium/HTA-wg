## R RESOURCES

JB Rickert
September 24, 2024

## Introduction
This document is a first draft of what is intended to be a relatively short list of R resources useful for health technology assessment. **It has not been reviewed by the working group.**


## R Packages

## Decision Analytics 

[rdecision](https://cran.r-project.org/package=rdecision)  v1.2.1: Provides classes and functions for modelling health care interventions using decision trees and semi-Markov models. Mechanisms are provided for associating an uncertainty distribution with each source variable and for ensuring transparency of the mathematical relationships between variables. The package terminology follows *Decision Modelling for Health Economic Evaluation*, [Briggs et al.(2006)](https://www.alibris.com/search/books/isbn/9780198526629?invid=18049473001&utm_source=Google&utm_medium=cpc&utm_campaign=NMPi&gad_source=1&gclid=Cj0KCQjwxsm3BhDrARIsAMtVz6OavWtY5J0Z_4FeZnqoQCnrlrJvEZ3ieQSafj1wgRa8Fp50ecUbtY4aAquJEALw_wcB&gclsrc=aw.ds).


### General

[NHANES](https://cran.r-project.org/package=NHANES) v2.1.0: Body Shape and related measurements from the US National Health and Nutrition Examination Survey ([NHANES, 1999-2004](https://www.cdc.gov/nchs/nhanes/index.htm?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fnchs%2Fnhanes.htm)). 

[phsmethods](https://cran.r-project.org/package=phsmethods) v1.02: A collection of methods for commonly undertaken analytical tasks, primarily developed for Public Health Scotland (PHS) analysts, but the package is also generally useful to others working in the healthcare space, particularly since it has functions for working with Community Health Index (CHI) numbers. 

### Health Care Economics

[eqSd](https://cran.r-project.org/package=eq5d) v0.15.4: EQ-5D is a health related quality of life instrument developed by the [EuroQol group](https://euroqol.org/) and used in the clinical and economic evaluation of health care. The eq5d package provides methods to calculate index scores from a subject's dimension scores as well as methods for the analysis of EQ-5D profiles, and also provides a shiny app to enable the calculation, visualisation and automated statistical analysis of EQ-5D data via a web browser using EQ-5D dimension scores stored in CSV or Excel files.

[eq5dsuite](https://cran.r-project.org/package=eq5dsuite) v1.0.0:  Enables users to calculate utility index values for the EQ-5D instruments, including crosswalk utilities using the original crosswalk developed by [van Hout et al. (2012)](https://www.valueinhealthjournal.com/article/S1098-3015(12)00058-7/fulltext?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS1098301512000587%3Fshowall%3Dtrue) which maps EQ-5D-5L responses to EQ-5D-3L index values, or the recently developed reverse crosswalk by [van Hout et al. (2021)](https://www.valueinhealthjournal.com/article/S1098-3015(21)00170-4/fulltext?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS1098301521001704%3Fshowall%3Dtrue) which maps EQ-5D-3L responses to EQ-5D-5L index values.. Users are allowed to add and/or remove user-defined value sets. Additional tools allow users to analyze EQ-5D data according to the recommended guidelines outlined in *Methods for Analyzing and Reporting EQ-5D data* by [Devlin et al. (2020)](https://link.springer.com/book/10.1007/978-3-030-47622-9).

[heemod](https://cran.r-project.org/package=heemod) v1.0.2: Implements the modelling and reporting features described in *Decision Modelling for Health Economic Evaluation* [Briggs, Andrew, et al. (2011)] and ; Siebert, U. et al. *State-Transition Modeling*. Medical Decision Making (2012)). It includes deterministic and probabilistic sensitivity analysis, heterogeneity analysis, time dependent state-time models such as semi-Markov and non-homogeneous Markov models.

[heRoMod](https://github.com/PolicyAnalysisInc/heRoMod) is a fork of heemod built on the web-based [heRo]() platform.

[hesim](https://cran.r-project.org/package=hesim) v0.5.5: Implements a modular and computationally efficient algorithms for parameterizing, simulating, and analyzing health economic simulation models inclusing cohort discrete time state transition models [Briggs et al. (1998)](https://link.springer.com/article/10.2165/00019053-199813040-00003), N-state partitioned survival models [Glasziou et al. (1990)](https://onlinelibrary.wiley.com/doi/10.1002/sim.4780091106), and individual-level continuous time state transition models [Siebert et al. (2012)](https://www.valueinhealthjournal.com/article/S1098-3015(12)01654-3/fulltext?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS1098301512016543%3Fshowall%3Dtrue), encompassing both Markov (time-homogeneous and time-inhomogeneous) and semi-Markov processes. Decision uncertainty from a cost-effectiveness analysis is quantified with standard graphical and tabular summaries of a probabilistic sensitivity analysis Claxton et al. (2005)](https://onlinelibrary.wiley.com/doi/10.1002/hec.985), and  [Barton et al. (2008)](https://www.valueinhealthjournal.com/article/S1098-3015(10)60568-2/pdf?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS1098301510605682%3Fshowall%3Dtrue).


[KHQ](https://cran.r-project.org/package=KHQ) v0.2.0: The King's Health Questionnaire (KHQ) is a disease-specific, self-administered questionnaire designed specific to assess the impact of Urinary Incontinence (UI) on Quality of Life. This package provides methods to calculate scores for each dimension of the KHQ; converts KHQ item scores to KHQ5D scores; and also calculates the utility index of the KHQ5D.

[valueEQ5D](https://cran.r-project.org/package=valueEQ5D) v0.7.2: Allows the calculation of both of EQ-5D (EQ-5D-3L and EQ-5D-5L) system scores and convert them to country specific index value scores. The package can also be used to map 5L scores to 3L index values for 10 countries. The value set and method for mapping follow [Van Hout et al (2012)](https://www.valueinhealthjournal.com/article/S1098-3015(12)00058-7/fulltext?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS1098301512000587%3Fshowall%3Dtrue).

### Meta Analysis

[esc](https://cran.r-project.org/package=esc) v0.5.1: Implementation of the web-based [Practical Meta-Analysis Effect Size Calculator](https://www.campbellcollaboration.org/research-resources/effect-size-calculator.html) from David B. Wilson, Effect size can be returned as standardized mean difference, Cohen's f, Hedges' g, Pearson's r or Fisher's transformation z, odds ratio or log odds, or eta squared effect size.

[mada](https://cran.r-project.org/package=mada) v0.5.11: Provides functions for diagnostic meta-analysis. Next to basic analysis and visualization the bivariate Model of Reitsma et al. (2005) that is equivalent to the HSROC of Rutter & Gatsonis (2001) can be fitted. A new approach based to diagnostic meta-analysis of Holling et al. (2012) is also available. Standard methods like summary, plot and so on are provided.

[meta](https://cran.r-project.org/package=meta) v7.0-0: User-friendly general package providing standard methods for meta-analysis and supporting Schwarzer, Carpenter, and Rücker , *Meta-Analysis with R* [Schwarzer et al. (2015)](https://link.springer.com/book/10.1007/978-3-319-21416-0) including: 

- common effect and random effects meta-analysis
- several plots (forest, funnel, Galbraith / radial, L'Abbe, Baujat, bubble) 
- three-level meta-analysis model 
- generalised linear mixed model 
- Hartung-Knapp method for random effects model 
- Kenward-Roger method for random effects model 
- prediction interval
- statistical tests for funnel plot asymmetry
- trim-and-fill method to evaluate bias in meta-analysis
- meta-regression
- cumulative meta-analysis and leave-one-out meta-analysis
- import data from 'RevMan 5'
- produce forest plot summarising several (subgroup) meta-analyses.

[metaBMA](https://cran.r-project.org/package=metaBMA) v0.6.9: Computes the posterior model probabilities for standard meta-analysis models (null model vs. alternative model assuming either fixed- or random-effects, respectively). These posterior probabilities are used to estimate the overall mean effect size as the weighted average of the mean effect size estimates of the random- and fixed-effect model as proposed by [Gronau et al. (2017)](https://www.tandfonline.com/doi/full/10.1080/23743603.2017.1326760). The user can define a wide range of non-informative or informative priors for the mean effect size and the heterogeneity coefficient. Moreover, using pre-compiled Stan models, meta-analysis with continuous and discrete moderators with Jeffreys-Zellner-Siow (JZS) priors can be fitted and tested. This allows to compute Bayes factors and perform Bayesian model averaging across random- and fixed-effects meta-analysis with and without moderators. For a primer on Bayesian model-averaged meta-analysis, see [Gronau wt al. (2021)](https://journals.sagepub.com/doi/10.1177/25152459211031256).

[metadat](https://cran.r-project.org/package=metadat) v1.2.0: A collection of meta-analysis datasets for teaching purposes, illustrating/testing meta-analytic methods, and validating published analyses

[metafor](https://cran.r-project.org/package=metafor) v4.6.0: A comprehensive collection of functions for conducting meta-analyses in R including functions to calculate various effect sizes or outcome measures, mixed-effects models, meta-regression analyses, meta-analytical plots, generalized linear (mixed-effects) models, functions to fit meta-analytic multivariate/multilevel models that account for non-independent sampling errors, and network meta-analyses. See [Viechtbauer (2010)](https://www.jstatsoft.org/article/view/v036i03) for an introduction. 

[mixmeta](https://cran.r-project.org/package=mixmeta) v1.2.0: A collection of functions to perform various meta-analytical models through a unified mixed-effects framework, including standard univariate fixed and random-effects meta-analysis and meta-regression, and non-standard extensions such as multivariate, multilevel, longitudinal, and dose-response models. 

[netmeta](https://cran.r-project.org/package=netmeta) v2.9-0: Implements a comprehensive set of frequentist methods for network meta-analysis including:

- additive network meta-analysis for combinations of treatments
- network meta-analysis of binary data using the Mantel-Haenszel or non-central hypergeometric distribution method
- rankograms and ranking of treatments by the Surface under the cumulative ranking curve (SUCRA)
- ranking of treatments using P-scores
- split direct and indirect evidence to check consistency
- league table with network meta-analysis results
- 'comparison-adjusted' funnel plots
- net heat plot and design-based decomposition of Cochran's Q
- measures characterizing the flow of evidence between two treatments
- automated drawing of network graphs
- partial order of treatment rankings ('poset') and Hasse diagrams 
- contribution matrix 

[mvmeta](https://cran.r-project.org/package=mvmeta) v1.0.3: Collection of functions to perform fixed and random-effects multivariate and univariate meta-analysis and meta-regression.

[rmeta](https://cran.r-project.org/package=rmeta) v3.0: Functions for simple fixed and random effects meta-analysis for two-sample comparisons and cumulative meta-analyses. Draws standard summary plots, funnel plots, and computes summaries and tests for association and heterogeneity.

### Survival Analysis

[easysurv](https://cran.r-project.org/web/packages/easysurv/index.html#:~:text=https%3A//CRAN.R%2Dproject.org/package%3Deasysurv) v2.0.1: Inspect survival data, plot Kaplan-Meier curves, assess the proportional hazards assumption, fit parametric survival models, predict and plot survival and hazards, and export the outputs to Excel. A simple interface for fitting survival models using `flexsurv`.

[flexsurv](https://cran.r-project.org/package=flexsurv) v2.3.2: Flexible parametric models for time-to-event data, including the Royston-Parmar spline model, generalized gamma and generalized F distributions. Any user-defined parametric distribution can be fitted, given at least an R function defining the probability density or hazard. There are also tools for fitting and predicting from fully parametric multi-state models, based on either cause-specific hazards or mixture models.


## Tutorials

[How to perform a meta-analysis with R: a practical tutorial](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10231495/pdf/ebmental-2019-300117.pdf) Sara Balduzzi, Gerta Rücker, and Guido Schwarzer


[Systematic Review and Meta-analysis of Diagnostic and Prognostic Studies: a Tutorial](https://www.scielo.br/j/abc/a/fM7by9YHVXjb3GbdnnMcdJv/?format=pdf&lang=en) Marcos R. de Sousa1 and  Antonio Luiz Ribeiro1

[Tidy Modeling with R](https://www.tmwr.org/);: Max Kuhn and Julia Silge

[Tutorial for performing systematic review and meta-analysis with interventional anesthesia studies](https://pubmed.ncbi.nlm.nih.gov/30717891/) by Barbosa et al. 


