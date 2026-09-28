# ECON 4420: Applied Data Analysis for Tackling Economic Problems

**Columbia University, Department of Economics · Spring 2027**

*DRAFT. Items in [brackets] are placeholders.*

| | |
|---|---|
| **Instructor** | Michael Carlos Best · mcb2270@columbia.edu |
| **Meetings** | Mondays & Wednesdays, [Time] (75 minutes) · [Room] |
| **Office hours** | [Time / place / sign-up link] |
| **Teaching assistants** | [Names, emails, sections] |
| **Course repository** | https://github.com/ECON4420-AppliedDataAnalysis/ECON4420-class-materials |
| **Discussion / announcements** | [Ed / Courseworks] |

---



## Course description

In this class we will learn how to deploy the tools you have learned in micro, macro, and econometrics to study some of the most important economic problems facing society. We will leverage newly available large datasets and the tools of modern empirical economics and data science to study topics such as: economic opportunity, education, racial disparities, health, criminal justice, the environment, and development. 

In micro, macro, and econometrics, you primarily a) saw the tools of economics as abstract tools that you _could_ apply to economic problems; and b) saw the final outputs but not how the sausage was made. In this class we'll seek to teach economics much more like a bench science: We want you to learn how to _do_ economics rather than "just" how to digest the economics that other people have done. 



Two features set it apart.

First, it builds on your prior coursework in micro, macro, and econometrics. We will work with the underlying research designs (difference-in-differences, regression discontinuity, instrumental variables, randomized experiments, and machine-learning prediction) rather than only the headline findings.

Second, it assumes you have access to AI tools, and it raises expectations to match. Work that once took a semester (building a new dataset, replicating a published result, or benchmarking a prediction model) is now within reach of a group of undergraduates in a couple of weeks. You will be graded on the quality of the economics and the evidence: good questions, credible designs, careful checks, and clear communication.

**Acknowledgements.** This course draws heavily on *Using Big Data to Solve Economic and Social Problems* by Raj Chetty and Greg Bruich (Harvard Econ 50 / Stanford Econ 45), on Kyle Coombs's *Big Data and Economics* (Bates College ECON/DCS 368), and on *Data Science for Economists* (UC Berkeley Econ 148). I am grateful to their instructors for making their materials publicly available.

## Prerequisites

- ECON UN3211 Intermediate Microeconomics
- ECON UN3213 Intermediate Macroeconomics
- ECON UN3412 Introduction to Econometrics

No prior programming experience beyond what you used in Econometrics is required. We teach the course in **R** and **Stata**. That means that we have TA support for debugging your code in **R** or **Stata**. You may use **Python** if you prefer, but then this will mean that the TAs may not be able to help you debug your code.



---

## How the course works: GitHub

The course is run primarily out of GitHub. The course repository holds the syllabus, lecture slides, code, data links, and exercise instructions. Exercises are distributed and submitted through **Codio**, which you can reach from [Courseworks]. Each group works in a shared Codio workspace backed by a private group GitHub repository, and the state of that repository at the deadline is your submission. [Confirm how Codio group projects and GitHub sync are set up.]

The first two weeks include hands-on Git and GitHub instruction. By the end of Week 2 every student should be able to clone a repository, commit, push, open a pull request, and resolve a merge conflict. Before the first class, please:

1. Create a GitHub account (use your Columbia email, or add it to your account).
2. Install Git, plus R and/or Stata [version/license info] (or Python). You can work in RStudio or VS Code for R, in Stata's own interface or VS Code for Stata, and in VS Code for Python.
3. Read chapters [X–Y] of Jenny Bryan, *Happy Git and GitHub for the useR* (https://happygitwithr.com).

**Repository layout**

```
/syllabus        syllabus.md and syllabus.pdf
/lectures        slides and lecture code, by week
/exercises       instructions and starter code for Exercises 1–5
/data            small datasets, plus links and download scripts for large ones
/resources       Git guides, R/Stata references, AI-use guidance
```

---

## Assessment

| Component | Weight |
|---|---|
| Exercises 1–4 (group) | 25% |
| Exercise 5: Prediction Hackathon (group) | 15% |
| Midterm exam (individual), Wed Mar 10 | 20% |
| Final exam (individual) | 20% |
| Individual reflections (one per exercise) | 10% |
| Participation (in-class activities, Git check-ins) | 10% |

### Groups

You will work in groups of **4**. Groups are assigned at random for each exercise, including the hackathon, so you will work with different classmates throughout the term. If enrollment does not divide evenly by 4, some groups will have 3 or 5 members. Every group member is expected to contribute to the code, analysis, and writing, and the commit history in your group repository should reflect that.

**Peer evaluations.** After each exercise, every student submits a short confidential peer evaluation. Individual grades on group work may be adjusted, up or down, based on peer evaluations and repository contribution history.

### Individual reflections

Within 48 hours of each exercise deadline, each student submits a one-page individual reflection covering what you personally did, the most important thing you learned, one thing your group got wrong or would do differently, and how you used AI tools (see the AI policy).

### Presentations

After every exercise, including the hackathon, the class following the deadline is a presentation session (a Monday for Exercises 1–4, and Wednesday, Apr 28 for the hackathon). **Seven groups, selected at random at the start of class, present**: 6 minutes of presentation plus 4 minutes of questions. Because any group may be selected, every group must submit slides with the exercise and be ready to present. The version committed at the deadline is the one you present. Any group member may be asked to answer any question, so every member should understand every part of the submission.

---

## Data exercises

Exercises 1–4 are due at **11:59 pm on the Sunday** before the presentation session. The hackathon is due at **11:59 pm on Tuesday, Apr 27**.

| # | Exercise | Skills | Released | Due | Presented |
|---|---|---|---|---|---|
| 1 | **Describing Opportunity:** mapping and describing intergenerational mobility with the Opportunity Atlas | Git workflow, data cleaning and merging, visualization, binned scatter plots, regression | Wed Jan 27 | Sun Feb 7 | Mon Feb 8 |
| 2 | **Building New Data: Text and Polarization:** building a dataset from political text and measuring how polarization in US political speech has changed over time | APIs, scraping, text as data, AI-assisted data extraction and validation | Mon Feb 8 | Sun Feb 21 | Mon Feb 22 |
| 3 | **Experiments:** replicating and extending a randomized evaluation of cash transfers | Treatment effects, balance, power calculations, pre-registration | Mon Mar 22 | Sun Apr 4 | Mon Apr 5 |
| 4 | **Natural Experiments:** replicating and extending a quasi-experimental study | Regression, DiD / event study, regression discontinuity, clustering, robustness | Mon Apr 5 | Sun Apr 18 | Mon Apr 19 |
| 5 | **Prediction Hackathon** (see below) | Machine learning, cross-validation, regularization, out-of-sample evaluation | Mon Apr 19 | Tue Apr 27 | Wed Apr 28 |

**Every exercise includes** a group repository containing code that runs end-to-end, a README explaining how to reproduce every result, a short written report [page limit], and an AI-use log (see the AI policy).

**The bar is higher than in a course without AI.** Clean, working code is the minimum. Grades reflect the quality of the question, the credibility of the design, the checks you ran to convince yourselves the results are right, and the clarity of the write-up.

### Exercises 2–4: paper options

**Exercise 2: Building New Data: Text and Polarization.** Your group will build a new dataset of US political speech and use it to describe how political polarization has changed over time. Choose one of two routes:

- **Update Gentzkow, Shapiro & Taddy (2019).** Extend their measure of partisanship in congressional speech past the end of their sample, using the Congressional Record, and document what has happened since.
- **Social media speech.** Collect posts by US politicians and document how their language has changed over time. [X/Twitter API read access is now paid and the free academic tier has been discontinued. Confirm a feasible source before release, e.g., Bluesky's open API or an existing archive.]

**Exercise 3: Experiments.** Your group will replicate the main results of one of the following papers and then extend them:

- Vivalt, Rhodes, Bartik, Broockman, Krause & Miller (2024), on the effects of a guaranteed income in the United States.
- Egger, Haushofer, Miguel, Niehaus & Walker (2022), *Econometrica*, on the general equilibrium effects of cash transfers in Kenya.

**Exercise 4: Natural Experiments.** Your group will replicate the main results of one of the following papers and then extend them:

- Marx, Pons & Rollet (2024), "Electoral Turnovers," *Review of Economic Studies*, a close-elections regression discontinuity design. [Paper](https://vrollet.github.io/files/Electoral_Turnovers_published.pdf) · [Replication package](https://zenodo.org/records/13314638)
- Akcigit, Grigsby, Nicholas & Stantcheva (2022), "Taxing Innovation in the Twentieth Century," *Quarterly Journal of Economics*, on the effects of taxes on innovation. [Replication package](https://dataverse.harvard.edu/file.xhtml?fileId=4750835&version=1.1)

### Exercise 5: Prediction Hackathon

Your group will build a model to predict an economically interesting outcome, such as [upward mobility for small geographic units from Opportunity Atlas and Census covariates]. The teaching staff hold back the outcomes for a test sample. Groups submit predictions on the test sample, which are scored automatically and posted to a class leaderboard.

Grades are based on:

- **Out-of-sample performance** on the held-out test set [X%]
- **Economics:** interpretation of which features matter and why, plus what the model should and should not be used for [X%]
- **Reproducibility and code quality** [X%]
- **Presentation** on Wed Apr 28, for the groups selected to present [X%]

Leaderboard rank is only one part of the grade. A thoughtful, well-understood model that places in the middle of the leaderboard can earn a top grade.

---

## Schedule

*Readings are listed by author and year. Full citations and links are on the course repository. Topics and dates may shift.*

| # | Date | Topic | Readings / notes |
|---|---|---|---|
| 1 | Wed Jan 20 | Why big data? Course overview; the geography of opportunity and the "fading American dream" | Chetty, Hendren, Kline & Saez (2014); Chetty et al. (2017), *Science* · Set up GitHub and software before next class |
| 2 | Mon Jan 25 | **Git & GitHub I:** repositories, commits, push/pull; getting started in Codio · **Ex 1 groups assigned** | *Happy Git with R* · Bring laptops |
| 3 | Wed Jan 27 | **Git & GitHub II:** branches, pull requests, merge conflicts, group workflow; reproducible projects in R and Stata · **Ex 1 released** | *Happy Git with R* · Bring laptops |
| 4 | Mon Feb 1 | Describing data: the Opportunity Atlas, binned scatter plots, visualization | Chetty, Friedman, Hendren, Jones & Porter (2018), "The Opportunity Atlas" |
| 5 | Wed Feb 3 | Neighborhoods and mobility I: Moving to Opportunity | Chetty, Hendren & Katz (2016) |
| | *Sun Feb 7* | ***Ex 1 due*** | |
| 6 | Mon Feb 8 | **Ex 1 presentations** · **Ex 2 released** | |
| 7 | Wed Feb 10 | Neighborhoods and mobility II: movers designs and exposure effects; working with AI coding tools | Chetty & Hendren (2018a) |
| 8 | Mon Feb 15 | Building new data: APIs, scraping, text as data, and LLMs for data extraction; measuring polarization in political speech | Gentzkow, Kelly & Taddy (2019); Dell (2025), *JEL*; Gentzkow, Shapiro & Taddy (2019), *Econometrica* |
| 9 | Wed Feb 17 | Development: measuring poverty with phones and satellites | Blumenstock, Cadamuro & On (2015); Jean et al. (2016) |
| | *Sun Feb 21* | ***Ex 2 due*** | |
| 10 | Mon Feb 22 | **Ex 2 presentations** | |
| 11 | Wed Feb 24 | Education I: measuring teacher impacts | Chetty, Friedman & Rockoff (2014a, b) |
| 12 | Mon Mar 1 | Education II: colleges and mobility | Chetty, Friedman, Saez, Turner & Yagan (2020) |
| 13 | Wed Mar 3 | Racial disparities in economic opportunity | Chetty, Hendren, Jones & Porter (2020) |
| 14 | Mon Mar 8 | Midterm review | |
| 15 | Wed Mar 10 | **Midterm exam** | |
| | Mar 15–19 | ***Spring recess (no class)*** | |
| 16 | Mon Mar 22 | Experiments: RCTs, balance, power; cash transfers and general equilibrium effects · **Ex 3 released** | [Experiments reading]; Egger et al. (2022), *Econometrica*; Vivalt et al. (2024) |
| 17 | Wed Mar 24 | Criminal justice: judge-assignment designs and IV | Dobbie, Goldin & Yang (2018) |
| 18 | Mon Mar 29 | Health: income and life expectancy; health insurance experiments | Chetty et al. (2016), *JAMA*; Finkelstein et al. (2012) |
| 19 | Wed Mar 31 | Taxation and behavioral economics: the EITC and retirement savings | Chetty, Friedman & Saez (2013); Chetty et al. (2014) |
| | *Sun Apr 4* | ***Ex 3 due*** | |
| 20 | Mon Apr 5 | **Ex 3 presentations** · **Ex 4 released** | |
| 21 | Wed Apr 7 | Methods: difference-in-differences and event studies (and recent critiques) | [DiD survey reading] |
| 22 | Mon Apr 12 | Methods: regression discontinuity | [RDD reading] |
| 23 | Wed Apr 14 | Environment: pollution and health | Currie & Walker (2011) |
| | *Sun Apr 18* | ***Ex 4 due*** | |
| 24 | Mon Apr 19 | **Ex 4 presentations** · **Ex 5 (Hackathon) released** | |
| 25 | Wed Apr 21 | Prediction I: prediction policy problems; regularization and cross-validation | Kleinberg, Ludwig, Mullainathan & Obermeyer (2015); Mullainathan & Spiess (2017) |
| 26 | Mon Apr 26 | Prediction II: trees and forests, heterogeneous effects, and algorithmic bias | Wager & Athey (2018); Obermeyer et al. (2019) |
| | *Tue Apr 27* | ***Ex 5 (Hackathon) due*** | |
| 27 | Wed Apr 28 | **Hackathon presentations and final leaderboard** | |
| 28 | Mon May 3 | Final exam review; course wrap-up | Last day of classes |
| | [Finals] | **Final exam** [date and time set by the Registrar] | |

---

## Policy on AI tools

AI tools, including chat assistants and agentic coding tools such as Claude Code, Cursor, and GitHub Copilot, are **allowed and encouraged** in this course. Learning to use them well is one of the course's goals.

1. **You own everything you submit.** "The AI did it" is never an explanation for an error. Any group member may be asked to explain any line of code or any number in your report, both in presentations and in grading.
2. **Document your use.** Each exercise repository must include an `AI_LOG.md` briefly describing which tools you used, for what, and where they got something wrong that you caught. Honest, specific logs are rewarded; they are not penalized.
3. **Verify.** AI tools can invent citations, variables, and results. Check every citation, and confirm that the data and code actually produce every reported number.
4. **Expectations are calibrated to AI access.** Exercises are designed assuming you have these tools. A submission that would have been excellent without AI may be average in this course.
5. **Individual reflections and peer evaluations are your own.** Write these without AI assistance.

## Other policies

**Late work.** [e.g., each group has X late days for the term; after that, Y% per day.]

**Academic integrity.** Collaboration within your group is expected. Sharing code or results between groups is not allowed except in designated collaborative activities. Undisclosed AI use, or submitting work you cannot explain, violates the course AI policy. See [Columbia academic integrity policy link].

**Accessibility.** [Columbia Disability Services statement and link.]

**Data use.** Some datasets carry use agreements. Follow them, and do not commit restricted data to GitHub.

---

*This syllabus is maintained as `syllabus/syllabus.md` in the course repository, and a PDF copy is generated from it. The GitHub version is authoritative.*
