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
* Seminar leader: [Dr. Michael Ganslmeier](mailto:m.g.ganslmeier@lse.ac.uk), Methodology.
* GTA (no office hours): [Pedro Torres-Lopez](mailto:p.torres-lopez@lse.ac.uk), Social Policy. 

Office hour may be booked via LSE's StudentHub. If you have questions or concerns about class material, problem sets, or the exam, please use the [class forum on Moodle](https://moodle.lse.ac.uk/mod/forum/view.php?id=1232310). We will not reply to emails about the course material, but we will reply promptly to questions posted on the forum. Of course, if you questions or concerns are of a private or personal nature, please do email or attend office hours. 

### Readings and textbooks

There is a reasonable amount of reading for this class, especially in the early weeks. You are strongly encouraged to do the reading **before class**, paying close attention to details (i.e., do not skim over equations). In addition to some key articles, throughout the term we will dip into three main textbooks, which we will refer to by their acronyms: 

* **MHE**: Angrist and Pischke, _Mostly Harmless Econometrics: An Empiricist's Companion_, 2009, Princeton University Press. 
* **CIS**: Imbens and Rubin, _Causal Inference for Statistics, Social, and Biomedical Sciences_, 2015, Cambridge University Press. 
* **TE** Huntington-Klein, _The Effect: An Introduction to Research Design and Causality_, 2022, CRC Press. 

If you are particularly interested in the course material, there will be additional readings set from the following textbooks (as well as a few articles): 

* **CMRI**: Pearl, _Causality: Models Reasoning and Inference (2nd Ed)_, 2009, Cambridge University Press.
* **CISAP**: Pearl, Glymour, and Jewell, _Causal Inference in Statistics: A Primer_, 2016, Wiley.
* **CIWI**: Hernan and Robins, _Causal Inference: What If_, 2020, Routledge. 

_Note_: if you are particularly interested in graphical models and their application to causal inference, it is strongly recommended that you do all the readings from either CMRI or CISAP. CMRI is extremely technical and dense, while CISAP is a gentler (though not that gentle) introduction to some of the basics introduced in CMRI. If there are suggested readings from both books, you should choose either, not both.

### Formative problem sets

Statistics is best learned by doing. Formative problem sets will be released every two weeks at 5pm, after seminar. You must submit one week later at 5pm, on **Moodle**. Your submission should be written in **RMarkdown**, and must be a **knitted .pdf**, formatted as shown in this [problem set template](psets/template/pset_template.Rmd). If you do not follow the formatting requirements your problem set will not be marked. Comments will be returned via Moodle within two weeks of submission. 

|  |  Type | Release date | Due date  |
|:--:|:-------:|:-----:|:-----|
| 1 | [Formative problem set 1](#problem-set-1) | 25 January 2023 - 5pm | 1 February 2023 - 5pm |
| 2 | [Formative problem set 2](#problem-set-2) | 8 February 2023 - 5pm | 15 February 2023 - 5pm  |
| 3 | [Formative problem set 3](#problem-set-3) | 29 February 2023 - 5pm | 7 March 2023 - 5pm  |
| 4 | [Formative problem set 4](#problem-set-4) | 14 March 2023 - 5pm  | 21 March 2023 - 5pm  |
| 5 | [Formative problem set 5](#problem-set-5) | 28 March 2023 - 5pm | 4 April 2023 - 5pm  |

### Quick links to lectures

| Week |  Topic |  
|:--:|:-------|
| 1  | [Causal Frameworks](#1-causal-frameworks) |   
| 2  | [Randomization](#2-randomization) | 
| 3  | [Selection on Observables 1](#3-selection-on-observables-1) | 
| 4  | [Selection on Observables 2](#4-selection-on-observables-2) | 
| 5  | [Selection on Observables 3](#5-selection-on-observables-3) | 
| 6  | _Reading week_ |  
| 7  | [Difference-in-Differences 1](#7-difference-in-differences-1) |
| 8  | [Difference-in-Differences 2](#8-difference-in-differences-2) | 
| 9  | [Synthetic Control Methods](#9-synthetic-control-methods) |  
| 10 | [Instrumental Variables](#10-instrumental-variables) |  
| 11 | [Regression Discontinuity](#11-regression-discontinuity) | 

### Quick links to seminars

| Week |  Topic | 
|:--:|:-------|
| 2  | [Causality and Randomization](#seminar-causality-and-randomization) |  
| 4  | [Selection on Observables](#seminar-selection-on-observables) |
| 7  | [Difference-in-Differences](#seminar-difference-in-differences) |
| 9  | [Instrumental Variables](#seminar-instrumental-variables) |  
| 11 | [Regression Discontinuity](#seminar-regression-discontinuity) | 

### Detailed course schedule

_Note:_ Links to slides and code will be updated/added in advance of each week's teaching.

#### 1. Causal Frameworks

This week begins with an introduction to the class, both substantively and administratively. 

We then introduce the potential outcomes framework, which will provide the technical foundations that are used throughout the rest of the class. We will also briefly introduce the graphical approach to causal inference. 

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

This week we will introduce the concept of randomization and its value for causal inference. We will discuss, at a high level, design, analysis, and inference in randomized experiments. 

##### Lecture

- [Lecture Slides - Randomization](slides/L2_randomization.pdf)

##### Seminar: Causality and Randomization

- [Seminar Paper](seminars/seminar1/MY457_seminar1_paper.pdf) 
- [Seminar Slides](seminars/seminar1/slides/MY457_intro_seminars.pdf)
- [Seminar Code](seminars/seminar1/coding/seminar1_randomized_experiments.Rmd)
- [Seminar Questions](seminars/seminar1/paper/MY457_seminar1_questions.pdf)

##### Readings
* MHE: Chapter 2
* CIS: Chapters 3 & 4
* TE: Chapters 7 & 8

##### Additional readings
* CISAP: Chapter 3 OR CMRI: Chapters 3 & 4 

##### Problem Set 1
- [Problem Set](psets/pset1/pset1.pdf)
- [Data](psets/pset1/how_to_elect_more_women.dta)

#### 3. Selection on Observables 1

This week we will depart from the safe shores of randomization, into the dangerous waters of observational research design. We will begin with a theoretical exploration of the selection on observables design -- its assumptions and identification results -- using both potential outcomes and graphical theory. 

We will then begin an extended discussion (which will continue next week and the week after) of estimation of causal estimands in this setting, focusing first on subclassification. **Update**: Please note that we did not cover subclassification in the lectures. You can still read the slides to see how it works, but it will not be examinable this year. 

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

This week we will consider the three core estimation strategies for selection-on-observables designs: matching (including propensity scores), weighting, and regression. 

##### Lecture

- [Lecture Slides - Selection on Observables 2](slides/L4_soo_part2.pdf)

##### Seminar: Selection on Observables

- [Seminar Paper](seminars/seminar2/paper.pdf) 
- [Group allocation](seminars/group_allocation_for_presentations.xlsx)
- [Seminar Code](seminars/seminar2/coding/)
- [Seminar Questions](seminars/seminar2/)

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
