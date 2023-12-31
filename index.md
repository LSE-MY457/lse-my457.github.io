---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---
  
<!-- ![LSE](images/lse-logo.jpg) -->
# MY457 Causal Inference for Observational and Experimental Studies
  
### Winter Term 2024
  
[Main course repo](https://github.com/LSE-MY457/lse-my457.github.io)

[Moodle page](https://moodle.lse.ac.uk/course/view.php?id=1111)

### Instructors

* Course convenor and lecturer: [Dr. Daniel de Kadt](mailto:d.n.de-kadt@lse.ac.uk), Department of Methodology.
* Seminar leader: [Dr. Michael Ganslmeier](mailto:m.g.ganslmeier@lse.ac.uk), Department of Methodology.
* GTA (no office hours): [Pedro Torres-Lopez](mailto:p.torres-lopez@lse.ac.uk), Department of Social Policy. 

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
| 1  | [Potential Outcomes](#1-potential-outcomes) |   
| 2  | [Randomization](#2-randomization) | 
| 3  | [Selection on Observables 1](#3-selection-on-observables-1) | 
| 4  | [Selection on Observables 2](#4-selection-on-observables-2) | 
| 5  | [Difference-in-Differences 1](#5-difference-in-differences-1) |
| 6  | _Reading week_ |  
| 7  | [Difference-in-Differences 2](#7-difference-in-differences-2) | 
| 8  | [Synthetic Control Methods](#8-synthetic-control-methods) |  
| 9  | [Instrumental Variables](#9-instrumental-variables) |  
| 10 | [Regression Discontinuity](#10-regression-discontinuity) | 
| 11 | [Machine Learning and Causal Inference](#11-machine-learning-and-causal-inference) |   

### Quick links to seminars

| Week |  Topic | 
|:--:|:-------|
| 2  | [Potential Outcomes and Randomization](#seminar-potential-outcomes-and-randomization) |  
| 4  | [Selection on Observables](#seminar-selection-on-observables) |
| 7  | [Difference-in-Differences](#seminar-difference-in-differences) |
| 9  | [Instrumental Variables](#seminar-instrumental-variables) |  
| 11  | [Regression Discontinuity](#seminar-regression-discontinuity) | 

### Detailed course schedule

_Note:_ Links to slides and code will be updated/added in advance of each week's teaching.

#### 1. Potential Outcomes

This week begins with an introduction to the class, both substantively and administratively. 

We then introduce the potential outcomes framework, which will provide the technical foundations that are used throughout the rest of the class. We will also briefly introduce the graphical approach to causal inference. 

##### Lecture

- [Lecture Slides](XXX)

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

- [Lecture Slides](XXX)

##### Seminar: Potential Outcomes and Randomization

- [Seminar Slides](XXX)
- [Seminar Code](XXX)

##### Readings
* MHE: Chapter 2
* CIS: Chapters 3 & 4
* TE: Chapters 7 & 8

##### Additional readings
* CISAP: Chapter 3 OR CMRI: Chapters 3 & 4 

##### Problem Set 1
- [Problem Set](psets/pset1/problem_set1.pdf)
- [Data](psets/pset1/data/...)
