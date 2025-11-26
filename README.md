# Mediation Analysis of DLPFC Function and Fluid Intelligence
---
## Project Overview 
Using **523 participants** from the *Cambridge Centre for Ageing and Neuroscience (Cam-CAN)* dataset, I assessed whether changes in the dorsolateral prefrontal cortex (DLPFC) mediates the relationship between age and declining fluid intelligence. 
<br/>
Using **R**, I performed:
+ Data cleaning and pre-processing
+ Regression modelling
+ Mediation analysis (Baron and Kenny approach)
+ Testing model assumptions
+ Model comparison using AIC
+ Robust standard errors to address heteroscedasticity
<br/>
The final output included a **2,000-word APA-formatted report**, along with APA-style figures created in R.
<br/>
The project was completed as part of a neuroscience-focused statistics course and demonstrates skills in statistical modeling, data analysis and presentation, scientific writing, and critical evaluation of methodology. The final report received a mark of 84%, placing me at the top of my cohort.
<br/>
<br/>
The full written report (PDF) and all R code (in an `.Rmd` notebook) are included in this repository.

### Key Findings
- **Fluid intelligence declines non-linearly with age** - decline in Gf accelerates with age.
- **Both cortical thickness and grey-matter volume of the DLPFC decrease with age**
- **Grey-matter volume** (GM), but *not* cortical thickness (CT), significantly predicts fluid intelligence scores.
- However, **neither CT nor GM mediated** the relationship between age and Gf.
- GM appears to act as an *independent contributor* to cognitive performance.
### Limitations and what I learned
This project was a valuable opportunity to deepen my understanding of statistical modeling in cognitive neuroscience. Several methodological limitations strengthened my understanding:
+ Cross-sectional mediation: I learned that mediation with age as the IV is theoretically inappropriate in cross-sectional designs due to the lack of temporal ordering. I now apply this principle when choosing statistical models.
+ Polynomial terms: I learned that squared predictors should be orthogonalised (e.g., polynomial expansion) to avoid multicollinearity.
+ Reporting exclusions: I improved my practice of clearly and explicitly documenting participant exclusions and preprocessing steps, which increases transparency and reproducibility.
### Tools and Packages
+ **R**
+ **tidyverse** (dplyr, ggplot2, tidyr)
+ **ggplot2**
+ **lmtest**
+ **car**
+ **sandwich**
+ **markdown**

### Statistical Techniques
- Outlier checks, VIF, heteroscedasticity tests (Breusch-Pagan)
- LOESS smoothing for visualisation
- Multiple linear regression
- Quadratic modelling
- Mediation pathway testing
- AIC model comparison
---
## Repository Structure
```text
data/
(data not included - Cam-CAN requires access permission
report/
neuroscience_report.pdf
code/
```
