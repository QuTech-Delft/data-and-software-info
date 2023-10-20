# Software Quality and Reproducible Software

## Why?

During your time at QuTech chances are high that you are going to write some piece of software. This could be a simple script to analyze your data, a python library you want to share with your fellow researchers or perhaps even some software you want to share with the outside world. For some of the software that you are going to write it is advantageous to have your software be reproducible.

Being mindful of software reproducibility can help you if you have encountered the following problems before:

* You wrote a script to analyze some data a few months ago, you now have new data. You can either no longer find the script or you can no longer get the script to work.
* You want to collaborate on research with other people. A vital script for the research only works on your laptop. You have been condemned to run the script for your colleagues for all of eternity.
* You finally got your script working. You barely dare to use your laptop to watch Netflix out of fear of breaking your script.
* You analyzed some data and started putting the results in your paper. While writing you notice some inconsistencies in the results, you dig into your script and find out it is not doing what you expected.

In general it will also make your research more valuable to QuTech and the research community:

* Making it easier to reproduce the results of your research
* Making it more transparent.
* Making it easier to re-use your work in other research. Your software can have a legacy within QuTech or the research community, even after you have finished your own research.

## How?

At QuTech we have defined a QuTech Software Maturity Model (QSMM) to help reason about software quality. The basic idea is that we define 4 maturity levels, depending on how the software will be used. For each level we define certain aspects which should be considered when developing software of this maturity level. To give an idea we show the levels with an example of what kind of software would fit this maturity:

| Level | Purpose | Examples |
|---|---|---|
| 1 - Prototype | One off scripts, only used by a single individual | Initial scripts used to explore your data. |
| 2 - Repeatable | Scripts for use within a group, scripts used for papers | Script used to perform data analysis for a paper, software for a piece of hardware only used in your group |
| 3 - Mature | Software used within multiple groups | Quantum Measurement Interface (QMI) |
| 4 - Defined | Software for use within and outside of QuTech | Quantum Inspire, Quantum Network Explorer |

We mostly want to focus here on level 1 and 2 because this is what most researchers will write at QuTech. If you do want to write software of higher levels you can of course ask the SDST for help!

Level 1 is intended for scripts that are only used by one individual just to for example quickly look through some newly generated data. With scripts of this category it is less important if there are some small bugs or if someone else cannot reproduce your results. They will most likely end up in the bin fairly quickly after being used.

A lot of research software also falls in category 2. With this software it is important that it can be reproduced. Whether that is by yourself when you want to run a similar or the same experiment again, or by someone else. Software that is used to actually run an experiment or analysis of data used in papers falls in this category. We often see that software that should have this maturity level is not actually easy to reproduce within QuTech. While making it reproducible often requires you to invest a little bit more time in the beginning of your project, we expect that throughout the duration of the project it will end up saving your time. We also provide you with some resources in the next section to get you started quickly.

## What?
<!---TODO: add relevant links-->

* Most software at QuTech is developed in Python. We provide some templates/examples to get you started on writing level 2 code in Python.

* There are also a few courses related to software development and reproducible software which can be followed for Graduate School Credits.

* For those that are interested in software quality in general this site also provides some info on a range of other topics and additional resources to learn more. 

* The SDST is also always available if you have questions about any of these topics or if need some help with using the templates for example.
