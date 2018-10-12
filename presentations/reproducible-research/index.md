---
title: "Data analysis best practice"
subtitle: "Reproducible research"
author: "Natalie Thurlby"
highlighter: highlight.js
hitheme: tomorrow
job: Data scientist, Jean Golding Institute
# logo: jgi-logo.jpg
mode: selfcontained
framework: io2012
url:
  assets: ../assets
  lib: ../librariesNew
widgets: mathjax
---




# Reproducible research
---

## What is reproducibility?

__Reproducible:__ Your research is reproducible if other people get the same results running the same analysis on your data.

__Replicabile:__ Your research replicates if other people repeat the experiment and their results are consistent with yours. 

Being reproducible is a prerequisite for being replicable; at a minimum your work should be reproducible. Good practices in data analysis will help you with both (and there are lots of other upsides to them which we'll discuss later).

---

## Reproducibility crisis

Less than 40% of replications of well-known Psychology studies had significant results:

![](fig/psychology-replication-paper.jpg.png)
"Open Science Collaboration. "Estimating the reproducibility of psychological science." Science 349.6251 (2015): aac4716.

Only 11% of replications of well-known cancer biology studies had significant results. 

Begley, C. Glenn, and Lee M. Ellis. "Drug development: Raise standards for preclinical cancer research." Nature 483.7391 (2012): 531.

---

## Most researchers think there is a problem with reproducibility

<center><img src="../../presentations/assets/img/reproducibility-intro/is-there-a-crisis.jpeg" height=400></center>
<center><font size = 2 >Baker, Monya. "1,500 scientists lift the lid on reproducibility." Nature News 533.7604 (2016): 452_</font></center>

---

## Most researchers have failed to reproduce a result

<center><img src="../../presentations/assets/img/reproducibility-intro/failed-to-reproduce.jpeg" height=400></center>
Of the scientists surveyed, __over 70% of scientists surveyed have experienced failure to reproduce other's results__ and __over 50% have failed to reproduce their own results__.

---

## Motivation

* It's the right thing to do - it gives us all better science.
* Helps you to avoid disaster/embarrassment.
* Saves you time in the long run
    * Helps you to write papers/your thesis.
    * Helps you continue your research by remembering what you did, so you or someone else can build on your previous work.
* Makes you a better researcher (because you know people can check your work, you will too)
* Good for your reputation (makes you more trustworthy). 

---
# Types of reproducibility problems

Next I'll introduce you to some bad analysis practices and how to avoid them. We'll practice this in the following sections and I'll give you a cheat sheet, so no need to memorise them (yet ;)).

---
## Data Storage

Avoid:
- Accidentally editing data or results
- Forgetting version or origin of data
- Storing your data in format which is hard for others to read

Bad because:
- Your results will probably be wrong. These kinds of problems have resulted in high-profile paper retractions, allegations of fraud, cancer trials based on results that can't be produced, etc.
- No one will be able to reproduce your results (including you), even if your results are "right".

Solve by:
- Organising your files neatly
- Setting data storage folders to read only
- Good naming conventions for files (no weird characters or spaces, descriptive, including important information) and explanation of those naming conventions if not obvious in the accompanying README.
- Include details of the origin, version, date downloaded, etc, of original data alongside the data in a README file.
- Store your data in text format - this is readable by everyone and easy to version control. 

---
## Analysis environment

Avoid:
- Clicking through a GUI to run analysis.
- Using proprietry software.
- Saving over earlier work without being able to get back to it and/or having files named "analysis_version32_final_actually_final.R"
- Forgetting what your scripts do.

Bad because:
- Will take you ages to repeat analysis if you need to.
- The order of doing things could change the results (results might be wrong).
- Other people will not be able to reproduce your work.
- Will take you forever to write up your work.

Solve by:
- Writing scripts
- Writing scripts in non-proprietry software (i.e. R and python beat STATA and SPSS)
- Using version control
- Make use of literate programming principles (easy with notebooks!)

---
## P-values

<center><font size=5>p < 0.05</font></center>
<center><img src="../../presentations/assets/img/reproducibility-intro/dice.jpeg" height=400></center>

---
## How often will we get a false positive?
* If we are testing one hypothesis?
* If we are testing 20?

---
## HARKing

HARKing = Hypothesising After Results are Known
<center><img src="../../presentations/assets/img/jellybean_xkcd.jpeg" height=100></center>

---
## P-hacking
<center><img src="../../presentations/assets/img/reproducibility-intro/p_values_xkcd.jpeg" height=400></center>

---
## Solutions to p-value problems
* Registered reports
* Multi-hypothesis corrections
* Try simulating your data

---
## Main causes of irreproducibility

1. Poor data storage
2. Poor analysis pipeline
3. Lack of sharing data/methods
4. Poor use of p-values

(1)-(3) are just a matter of becoming familiar with the tools we're going to be using today. If you have any more questions about (4), you can email us <ask-jgi@bristol.ac.uk>



