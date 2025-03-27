---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---
  
<!-- ![LSE](images/lse-logo.jpg) -->
<!-- # MY457 Causal Inference for Observational and Experimental Studies  -->
  
### Instructors

* Course convenor and lecturer: [Dr. Daniel de Kadt](mailto:d.n.de-kadt@lse.ac.uk), Methodology.
* Seminar leader: [Dr. Michael Schultz](mailto:m.schultz2@lse.ac.uk), Methodology.
* GTA (no office hours): [Pedro Torres-Lopez](mailto:p.torres-lopez@lse.ac.uk), Social Policy. 

Office hour may be booked via LSE's StudentHub. If you have questions or concerns about class material, problem sets, or the exam, please use the [class forum on Moodle](https://moodle.lse.ac.uk/mod/forum/view.php?id=1463342). We will generally not reply to emails about the course material, but we will reply promptly to questions posted on the forum. Of course, if you questions or concerns are of a private or personal nature, please email or attend office hours. 

### Readings and textbooks

There is a reasonable amount of reading for this class, especially in the early weeks. You are strongly encouraged to do the reading **before class**, paying close attention to details (i.e., do not skim over equations). In addition to some key articles, throughout the term we will dip into three main textbooks, which we will refer to by their acronyms: 

* **MHE**: Angrist and Pischke, _Mostly Harmless Econometrics: An Empiricist's Companion_, 2009, Princeton University Press. 
* **CIS**: Imbens and Rubin, _Causal Inference for Statistics, Social, and Biomedical Sciences_, 2015, Cambridge University Press. 
* **TE** Huntington-Klein, _The Effect: An Introduction to Research Design and Causality_, 2022, CRC Press. 

_Note_: The three textbooks have very different flavours, and are pitched at different technical levels. **MHE** is the classic graduate-level text for causal inference, and is challenging but very accessible, though now a little out of date as it was published in 2009. **CIS** is very dense and very technical, and serves as a reference text for much of the foundational material in the class (weeks 1-5). **TE** is the most accessible textbook and is very applied, while being lighter on details and generally less technically focused. The reading list is designed to allow you pick your own adventure, to a degree. 

If you are particularly interested in the course material, there will be additional readings set from the following textbooks (as well as a few articles): 

* **CMRI**: Pearl, _Causality: Models Reasoning and Inference (2nd Ed)_, 2009, Cambridge University Press.
* **CISAP**: Pearl, Glymour, and Jewell, _Causal Inference in Statistics: A Primer_, 2016, Wiley.
* **CIWI**: Hernan and Robins, _Causal Inference: What If_, 2020, Routledge. 

_Note_: if you are particularly interested in graphical models and their application to causal inference, it is strongly recommended that you do all the readings from either CMRI or CISAP. CMRI is extremely technical and dense, while CISAP is a gentler (though not that gentle) introduction to some of the basics introduced in CMRI. If there are suggested readings from both books, you should choose either, not both.

### Formative problem sets

Statistics is best learned by doing. There will be six problem sets, released at 5pm on Wednesdays. You must submit one weeks later at 11am, on **Moodle**. Your submission should be written in **RMarkdown**, and must be a **knitted .pdf**, formatted as shown in this [problem set template](psets/template/pset_template.Rmd), which produces a pdf that looks like [this](psets/template/pset_template.pdf). If you do not follow the formatting requirements your problem set will not be marked. Comments will be returned via Moodle within two weeks of submission. 

|  |  Type | Release date | Due date  |
|:--:|:-------:|:-----:|:-----|
| 1 | [Formative problem set 1](#problem-set-1) | 29 January 2025 - 5pm | 5 February 2025 - 11am |
| 2 | [Formative problem set 2](#problem-set-2) | 12 February 2025 - 5pm | 19 February 2025 - 11am  |
| 3 | [Formative problem set 3](#problem-set-3) | 5 March 2025 - 5pm | 12 March 2025 - 11am  |
| 4 | [Formative problem set 4](#problem-set-4) | 19 March 2025 - 5pm | 26 March 2025 - 11am  |
| 5 | [Formative problem set 5](#problem-set-5) | 2 April 2025 - 5pm  | 9 April 2025 - 11am  |

### Quick links to lectures

| Week |  Topic |  
|:--:|:-------|
| 1  | [Causal Frameworks](#1-causal-frameworks) |   
| 2  | [Randomization](#2-randomization) | 
| 3  | [Selection on Observables 1](#3-selection-on-observables-1) | 
| 4  | [Selection on Observables 2](#4-selection-on-observables-2) | 
| 5  | [Selection on Observables 3](#5-selection-on-observables-3) | 
| 6  | _Reading week_ |  
| 7  | [Instrumental Variables 1](#7-instrumental-variables-1) |  
| 8  | [Instrumental Variables 2](#8-instrumental-variables-2) |  
| 9  | [Regression Discontinuity](#9-regression-discontinuity) | 
| 10 | [Difference-in-Differences 1](#10-difference-in-differences-1) |
| 11 | [Difference-in-Differences 2](#11-difference-in-differences-2) | 

### Quick links to seminars

| Week |  Topic | 
|:--:|:-------|
| 2  | [Causality and Randomization](#seminar-causality-and-randomization) |  
| 4  | [Selection on Observables](#seminar-selection-on-observables) |
| 7  | [Instrumental Variables](#seminar-instrumental-variables) |  
| 9  | [Regression Discontinuity](#seminar-regression-discontinuity) | 
| 11 | [Difference-in-Differences](#seminar-difference-in-differences) |

### Detailed course schedule

_Note:_ Links to slides and code will be updated/added in advance of each week's teaching.

#### 1. Causal Frameworks

We begin with an introduction to the class, both substantively and administratively. 

We then introduce the potential outcomes framework, which will provide the technical foundations that are used throughout the rest of the class. We will also briefly introduce the graphical model for causal inference. 

##### Lecture

- [Lecture Slides - Introduction](slides/L1_intro.pdf)
- [Lecture Slides - Causal Frameworks](slides/L1_causalframeworks.pdf)

##### Readings
* MHE: Chapter 1
* CIS: Chapters 1, 2, and 3.1
* TE: Chapter 6 

##### Additional readings
* [Holland, P.W., 1986. Statistics and causal inference. _Journal of the American statistical Association_, 81(396), pp.945-960.](https://www.jstor.org/stable/2289064) (highly recommended)
* CISAP: Chapters 1 & 2 or CMRI: Chapters 1 & 2 
* TE: Chapters 1 & 2

#### 2. Randomization

We introduce the concept of randomization and its value for causal inference. We discuss, at a high level, design, analysis, and inference for randomized experiments. 

##### Lecture

- [Lecture Slides - Randomization](slides/L2_randomization.pdf)

##### Seminar: Causality and Randomization

- [Seminar Paper](seminars/seminar1/seminar1_paper.pdf) 
- [Seminar Questions](seminars/seminar1/seminar1_questions.pdf)
- [Seminar Code](seminars/seminar1/seminar1_experiments.Rmd)

##### Readings
* MHE: Chapter 2
* CIS: Chapters 3 & 4
* TE: Chapters 7 & 8

##### Additional readings
* CISAP: Chapter 3 OR CMRI: Chapters 3 & 4 

##### Problem Set 1
- [Problem Set](psets/pset1/pset1.pdf)
- [Data](psets/pset1/how_to_elect_more_women.dta)
- [Solution Set](psets/pset1/pset1_solutions.pdf)

#### 3. Selection on Observables 1

We depart from the safe shores of controlled randomization, into the treacherous waters of observational research design. We will begin with a theoretical exploration of the selection on observables design (SOO) -- its assumptions and identification results -- using both potential outcomes and graphical theory. 

##### Lecture

- [Lecture Slides - Selection on Observables 1](slides/L3_soo_part1.pdf)

##### Readings
* MHE: Chapter 3
* CIS: Chapters 12, 13, 18
* TE: Chapter 14

##### Additional readings
* [Cinelli, C., Forney, A., & Pearl, J. (2022). A Crash Course in Good and Bad Controls. Sociological Methods & Research](https://doi.org/10.1177/00491241221099552) (highly recommended)
* CISAP: Chapter 4 or CMRI: Chapter 5

#### 4. Selection on Observables 2

We consider the three most frequently seen estimation strategies for selection-on-observables designs: matching (including propensity scores), weighting, and regression. 

##### Lecture

- [Lecture Slides - Selection on Observables 2](slides/L4_soo_part2.pdf)

##### Seminar: Selection on Observables

- [Seminar Code](seminars/seminar2/seminar2_soo.Rmd)
- [Seminar Paper 1](seminars/seminar2/seminar2_paper1.pdf)
- [Seminar Paper 2 (response to paper 1)](seminars/seminar2/seminar2_paper2.pdf) 
- [Seminar Questions](seminars/seminar2/seminar2_questions.pdf)

##### Readings
* MHE: Sections 3.2 and 3.3
* CIS: Chapter 13
* TE: Chapter 14

##### Additional readings
* TE: Chapter 13 (gentler introduction to regression)
* [Lin, W. (2013). Agnostic Notes on Regression Aadjustments to Experimental Data: Reexamining Freedman’s Critique
. Annals of Applied Statistics](https://doi.org/10.1177/00491241221099552](https://projecteuclid.org/journals/annals-of-applied-statistics/volume-7/issue-1/Agnostic-notes-on-regression-adjustments-to-experimental-data--Reexamining/10.1214/12-AOAS583.full)https://projecteuclid.org/journals/annals-of-applied-statistics/volume-7/issue-1/Agnostic-notes-on-regression-adjustments-to-experimental-data--Reexamining/10.1214/12-AOAS583.full) (very technical but worth reading if interested in regression adjustment) 
* [Abadie, A. & Imbens, G. (2006). Large Sample Properties of Matching Estimators for Average Treatment Effects. Econometrica.](https://doi.org/10.1111/j.1468-0262.2006.00655.x) (if you want to understand matching bias -- very technical)
* [King, G. & Nielsen, R. (2019). Why Propensity Scores Should Not Be Used for Matching. Political Analysis.](https://doi.org/10.1017/pan.2019.11) (a critique of propensity score matching)

##### Problem Set 2
- [Problem Set](psets/pset2/pset2.pdf)
- [Data](psets/pset2/dollars_on_the_sidewalk.dta)
- [Solution Set](psets/pset2/pset2_solutions.pdf)

#### 5. Selection on Observables 3

We consider what happens if we are willing to weaken the assumptions underpinning our research designs, exploring partial identification and sensitivity analysis. 

##### Lecture

- [Lecture Slides - Selection on Observables 3](slides/L5_soo_part3.pdf)

##### Readings
* [Manski, C.F., 1990. Nonparametric bounds on treatment effects. The American Economic Review, 80(2), pp.319-323.](https://www.jstor.org/stable/2006592) (very technical but worth reading, even if only for the intuition.)
* [Imbens, G. W. (2003). Sensitivity to exogeneity assumptions in program evaluation. American Economic Review, 93(2), 126-132.](https://www.jstor.org/stable/3132212)
* [Cinelli, C., & Hazlett, C. (2020). Making sense of sensitivity: Extending omitted variable bias. Journal of the Royal Statistical Society Series B: Statistical Methodology, 82(1), 39-67.](https://academic.oup.com/jrsssb/article/82/1/39/7056023)

##### Additional readings
* [Rosenbaum, P. R., & Rubin, D. B. (1983). Assessing sensitivity to an unobserved binary covariate in an observational study with binary outcome. Journal of the Royal Statistical Society: Series B (Methodological), 45(2), 212-218.](https://www.jstor.org/stable/2345524) (technical but foundational)
* [Duarte, G., Finkelstein, N., Knox, D., Mummolo, J., & Shpitser, I. (2023). An automated approach to causal inference in discrete settings. Journal of the American Statistical Association, (just-accepted), 1-25.](https://www.tandfonline.com/doi/pdf/10.1080/01621459.2023.2216909) (very technical but very interesting)

#### 6. Reading Week

#### 7. Instrumental Variables 1

We now move onto a new research design: instrumental variables (IV). We introduce the basic architecture of modern IV, learn about the various assumptions needed to admit a causal interpretation, and explore some of the weaknesses and fragilities of the approach.

##### Lecture
- [Lecture Slides - Instrumental Variables 1](slides/L7_IV_part1.pdf)

##### Readings
* TE: Chapter 19
* MHE: Chapter 4 OR CIS: Chapters 23 and 24 

##### Additional readings
* [Deaton, A. (2010). Instruments, randomization, and learning about development. Journal of economic literature, 48(2), 424-455.](https://www.aeaweb.org/articles?id=10.1257/jel.48.2.424)
* [Imbens, G. W. (2010). Better LATE than nothing: Some comments on Deaton (2009) and Heckman and Urzua (2009). Journal of Economic literature, 48(2), 399-423.](https://www.aeaweb.org/articles?id=10.1257/jel.48.2.399)
* [Angrist, J. D., Imbens, G. W., & Rubin, D. B. (1996). Identification of causal effects using instrumental variables. Journal of the American statistical Association, 91(434), 444-455.](https://www.tandfonline.com/doi/abs/10.1080/01621459.1996.10476902)
* [Andrews, I., Stock, J. H., & Sun, L. (2019). Weak instruments in instrumental variables regression: Theory and practice. Annual Review of Economics, 11, 727-753.](annualreviews.org/doi/abs/10.1146/annurev-economics-080218-025643)

##### Seminar: Instrumental Variables

- [Seminar Paper](seminars/seminar3/seminar3_paper.pdf) 
- [Seminar Questions](seminars/seminar3/seminar3_questions.pdf)
- [Seminar Code](seminars/seminar3/seminar3_iv.Rmd)

##### Problem Set 3
- [Problem Set](psets/pset3/pset3.pdf)
- [Data](psets/pset3/foreign_aid_human_rights_and_democracy_promotion.dta)
- [Solution Set](psets/pset3/pset3_solutions.pdf)

#### 8. Instrumental Variables 2

Extending our investigation of IV designs, we focus on the interpertation and estimation of continuous IV settings, shift-share (Bartik) instruments, examiner designs, and recentered IV.

##### Lecture
- [Lecture Slides - Instrumental Variables 2](slides/L8_IV_part2.pdf)

##### Readings
* [Cunningham, S. (2021). Causal inference: The mixtape. Yale university press. Section 7.8.](https://mixtape.scunning.com/07-instrumental_variables)

##### Additional readings
* [Goldsmith-Pinkham, P., Sorkin, I., & Swift, H. (2020). Bartik instruments: What, when, why, and how. American Economic Review, 110(8), 2586-2624.](https://www.aeaweb.org/articles?id=10.1257/aer.20181047)
* [Borusyak, K., Hull, P., & Jaravel, X. (2022). Quasi-experimental shift-share research designs. The Review of Economic Studies, 89(1), 181-213.](https://academic.oup.com/restud/article-abstract/89/1/181/6294942)
* [Frandsen, B., Lefgren, L., & Leslie, E. (2023). Judging judge fixed effects. American Economic Review, 113(1), 253-277.](https://www.aeaweb.org/articles?id=10.1257/aer.20201860)

#### 9. Regression Discontinuity
We move to the next core research design, regression discontinuity (RD), considering modern approaches to both sharp and fuzzy RD settings.  We briefly consider the regression kink (RK) design.

##### Lecture
- [Lecture Slides - Regression Discontinuity](slides/L9_RDD.pdf)

##### Readings
* MHE: Chapter 6
* TE: Chapter 20
* [Cattaneo, M. D., & Titiunik, R. (2022). Regression discontinuity designs. Annual Review of Economics, 14, 821-851.](https://www.annualreviews.org/content/journals/10.1146/annurev-economics-051520-021409)

##### Additional readings
* [Lee, D. S., & Lemieux, T. (2010). Regression discontinuity designs in economics. Journal of economic literature, 48(2), 281-355.](https://www.jstor.org/stable/20778728) (strongly recommended)
* [Keele, L. J., & Titiunik, R. (2015). Geographic boundaries as regression discontinuities. Political Analysis, 23(1), 127-155.](https://www.cambridge.org/core/journals/political-analysis/article/geographic-boundaries-as-regression-discontinuities/2A59F3077F49AD2B908B531F6E458430)
* If very interested, see: 
  - Cattaneo, M. D., Idrobo, N., & Titiunik, R. (2020). A practical introduction to regression discontinuity designs: Foundations. Cambridge University Press.
  - Cattaneo, M. D., Idrobo, N., & Titiunik, R. (2024). A Practical Introduction to Regression Discontinuity Designs: Extensions. Cambridge: Cambridge University Press.

##### Seminar: Regression Discontinuity

- [Seminar Paper](seminars/seminar4/seminar4_paper.pdf) 
- [Seminar Questions](seminars/seminar4/seminar4_questions.pdf)
- [Seminar Code](seminars/seminar4/seminar4_rdd.Rmd)

##### Problem Set 4
- [Problem Set](psets/pset4/pset4.pdf)
- [Data](psets/pset4/pmgsy_working_aer_mainsample_reduced.dta)
- [Solution Set](psets/pset4/pset4_solutions.pdf)

#### 10. Difference-in-Differences 1

We now introduce one of the most popular research designs for applied causal inference, difference-in-differences (DiD). We consider cases in which a treatment is rolled out such that we have variation over two dimensions: _time_ and _units_. We focus almost exclusively on canonical cases in which we have only two time-periods and two treatment groups of units. We will close by briefly considering falsification tests in situations with two pre-treatment periods. Diverging from the previous approaches in which we rely on assumptions about the nature of treatment assignment, we introduce new assumptions about trends in potential outcomes over time. 

##### Lecture

- [Lecture Slides - Difference-in-Differences 1](slides/L10_DinD_part1.pdf)

##### Readings
* MHE: Section 5.2
* TE: Chapter 18

##### Additional readings
* [Card, D., & Krueger, A. B. (1993). (1994). Minimum Wages and Employment: A Case Study of the Fast-Food Industry in New Jersey and Pennsylvania. The American Economic Review, 84(4), 772-793.](https://davidcard.berkeley.edu/papers/njmin-aer.pdf) (foundational example)
* [Bertrand, M., Duflo, E., & Mullainathan, S. (2004). How much should we trust differences-in-differences estimates?. The Quarterly journal of economics, 119(1), 249-275.](https://academic.oup.com/qje/article-abstract/119/1/249/1876068) (classic focused on inference)
* [Roth, J. (2022). Pretest with caution: Event-study estimates after testing for parallel trends. American Economic Review: Insights, 4(3), 305-322.](https://www.aeaweb.org/articles?id=10.1257/aeri.20210236) (technical, focused on issues with pre-trend tests)

#### 11. Difference-in-Differences 2

We continue our exploration of DiD, broadening our focus to cases with more than 2 time periods. We discuss first the two-way fixed effects estimator that has been a dominant tool for estimating 'generalised difference-in-differences' and then explore the implied assumptions in this approach and its weaknesses, specifically for staggered and non-saturating treatments, and cases with heterogeneous treatment effects. We introduce alternative 'modern' estimators that are robust to these settings. We conclude with a very brief foray into the synthetic control method. 

##### Lecture

- [Lecture Slides - Difference-in-Differences 2](slides/L11_DinD_part2.pdf)

##### Readings
* [Baker, A. C., Larcker, D. F., & Wang, C. C. (2022). How much should we trust staggered difference-in-differences estimates?. Journal of Financial Economics, 144(2), 370-395.](https://www.sciencedirect.com/science/article/pii/S0304405X22000204) (has some quite accessible discussions)
* [Roth, J., Sant’Anna, P. H., Bilinski, A., & Poe, J. (2023). What’s trending in difference-in-differences? A synthesis of the recent econometrics literature. Journal of Econometrics.](https://doi.org/10.1016/j.jeconom.2023.03.008) (technical but a good overview)
* TE: Chapter 18, especially 18.3

##### Additional readings
* [Goodman-Bacon, A. (2021). Difference-in-differences with variation in treatment timing. Journal of Econometrics, 225(2), 254-277.](https://doi.org/10.1016/j.jeconom.2021.03.014) (very technical but parts can be read quite easily)
* [Callaway, B., & Sant’Anna, P. H. (2021). Difference-in-differences with multiple time periods. Journal of econometrics, 225(2), 200-230.](https://doi.org/10.1016/j.jeconom.2020.12.001)
* [Liu, L., Wang, Y., & Xu, Y. (2024). A practical guide to counterfactual estimators for causal inference with time‐series cross‐sectional data. American Journal of Political Science, 68(1), 160-176.](https://onlinelibrary.wiley.com/doi/full/10.1111/ajps.12723)
* [Dube, A., Girardi, D., Jorda, O., & Taylor, A. M. (2023). A local projections approach to difference-in-differences event studies (No. w31184). National Bureau of Economic Research.](https://www.nber.org/papers/w31184)
* [Abadie, A., (2021). Using synthetic controls: Feasibility, data requirements, and methodological aspects. Journal of economic literature, 59(2), pp.391-425.](https://www.aeaweb.org/articles?id=10.1257/jel.20191450)

##### Seminar: Difference-in-Differences

- [Seminar Code](seminars/seminar5/seminar5_did.Rmd)
- [Seminar Paper](seminars/seminar5/seminar5_paper.pdf) 
- [Seminar Questions](seminars/seminar5/seminar5_questions.pdf)

##### Problem Set 5
- [Problem Set](psets/pset5/pset5.pdf)
- [Data](psets/pset5/Norway-MSD.dta)
- [Solution Set](psets/pset5/pset5_solutions.pdf)


[COURSE ENDS]
