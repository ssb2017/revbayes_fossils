# RevBayes: Analysis of Fossil and Molecular Data

## Instructors: Tracy Heath, Walker Pett, and April Wright

### General Information
This workshop is a 3-hour session, held on January 8, 2017 at the [Society of Systematic Biologists Meeting in Baton Rouge, LA USA](https://ssb2017.github.io/). 

This half-day workshop will guide participants through the theory and practice of combined inference of dated phylogenies using fossil and molecular data. For this workshop, participants should attend the RevBayes Introduction workshop or have previous experience using RevBayes. We will cover the background necessary to understand the fossilized birth-death process, relaxed clock models, and discrete morphological evolution. The tutorial provided will demonstrate how to perform a "total-evidence analysis" on a provided dataset. Additionally, participants can bring their own data to analyze.  

### Travel Awards

[**Apply Here**](https://goo.gl/forms/9OkFAvmw1HApRLOs2)

The travel awards will be $400 each (for reimbursement of travel/registration to the conference) and preference will be given to students, early career scientists, and researchers working with natural history collections data.

To be eligible for an award, you must attend any TWO of the RevBayes workshops held at the SSB meeting. If one of those workshops is not the RevBayes Introduction, you must complete introductory materials that will be sent to you prior to the meeting (or demonstrate sufficient prior experience using RevBayes). 

Support for these travel awards is provided by funds from NSF grant DEB-1556615 (awarded to T. Heath, D. Ksepka, & R. Meredith) and NSF grant DEB-1355071 (J. Brown & R. Thomson)

## Required Background Material

This workshop covers a very complicated analysis that requires the participants to specify complex statistical models. Because of the challenging material, we expect all participants to have some previous experience using RevBayes before attending the workshop. This can be completed in two ways:

1. Attend the Introduction to RevBayes Workshop on Jan. 7 ([https://github.com/ssb2017/revbayes_intro](https://github.com/ssb2017/revbayes_intro))
2. Complete the introductory tutorials that are offered for the [introductory workshop](https://github.com/ssb2017/revbayes_intro):
	* Basic Introduction to Rev and MCMC ([tutorial PDF](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_Basics_Tutorial.pdf))
	* Substitution Models for Time-Constrained Trees ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_CTMC_Tutorial.pdf))
	* Partitioned Data Analysis ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_Partition_Tutorial.pdf))
	* *Optional*: Model Selection using Bayes Factors ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_BayesFactor_Tutorial.pdf))


## Install RevBayes

This workshop will use RevBayes v1.X. It can be downloaded from [revbayes.com](http://revbayes.github.io/code.html) for Windows 7 or higher or for Mac OSX 10.6 or higher. For Unix systems, you can clone the source code from [https://github.com/revbayes/revbayes](https://github.com/revbayes/revbayes).

## Accessory Programs

The RevBayes workshops will also use additional for analysis of output and summarization of the MCMC. Please download and install the following:

* Tracer ([http://tree.bio.ed.ac.uk/software/tracer/](http://tree.bio.ed.ac.uk/software/tracer/))
* FigTree ([http://tree.bio.ed.ac.uk/software/figtree/](http://tree.bio.ed.ac.uk/software/figtree/))
* IcyTree (a web-based tree viewer; [http://tgvaughan.github.io/icytree/](http://tgvaughan.github.io/icytree))
* Text editors
	* Mac OSX: [TextWrangler](http://www.barebones.com/products/TextWrangler/), [Sublime Text](https://www.sublimetext.com/)
	* Windows: [Notepad++](https://notepad-plus-plus.org/), [Sublime Text](https://www.sublimetext.com/)
	* Linux: [Geany](https://www.geany.org/), [Sublime Text](https://www.sublimetext.com/)

## Workshop Outline
### Background and Theory
The course will begin with lectures on the models and statistical methods for conducting a total-evidence analysis under the fossilized birth-death model in RevBayes. We will focus on the following models:

* Stochastic branching processes as tree priors, with particular emphasis on the fossilized birth-death model (FBD)
* Models of lineage-specific substitution rates (or rates of morphological change)
* Models of discrete morphological character change and accounting for acquisition biases

### Tutorial
After presenting the theoretical background, we will lead a hands-on tutorial using an empirical dataset. This exercise will demonstrate:

* Importing multiple data matrices in RevBayes
* Creating clade constraints
* Specification of the FBD model
* Sampling fossil occurrence dates from known age ranges
* Setting up the uncorrelated lognormal model for relaxing the molecular clock
* Defining the parameters of the GTR+G model of sequence evolution
* Applying a strict clock to the rates of morphological evolution
* Defining the parameters of the Mk model of discrete morphological character evolution while accounting for sampling only variable characters
* Executing an MCMC sampler in RevBayes
* Summarizing and evaluating the marginal posterior samples of various model parameters
* Summarizing a fossilized birth-death tree with sampled ancestors

The next section provides specific details for locating the tutorial exercise and associated files.

## Exercise: Total Evidence Analysis under the FBD Model in RevBayes

This tutorial is maintained on the RevBayes tutorial repository ([https://github.com/revbayes/revbayes_tutorial](https://github.com/revbayes/revbayes_tutorial)). On this site you can find a wide range of tutorials for different RevBayes analyses. 

### Download the Files

For this workshop, it is recommended that you create a working directory on your computer. You can call this `RB_TotalEvidence_FBD_Tutorial`.

In `RB_TotalEvidence_FBD_Tutorial` download the tutorial files and uncompress the zipped archives:

* [`data.zip`](link to zip)
* [`scripts.zip`](link to zip)

Also download the detailed tutorial document:

* [`RB_TotalEvidenceDating_FBD_Tutorial.pdf`](https://github.com/revbayes/revbayes_tutorial/blob/master/tutorial_TeX/RB_TotalEvidenceDating_FBD_Tutorial/RB_TotalEvidenceDating_FBD_Tutorial.pdf)

### Getting Started

Now that you have all the files and installed the software, execute RevBayes and follow the tutorial exercise. If you have any trouble, please ask for help. 