---
content_type: page
description: Instructions on setting up music21.
draft: false
title: 'Week 1: Setting Up Your Own Dev Environment'
uid: 7107b06f-f9da-4f59-a6ad-6bf1e899adb5
---
Until now, we used the Google `colab` notebook to quickly get started with computational music theory by doing everything on the web.

In developing your tools and solving your problems, you will need to be able to work on your development system on your computer. This page is my explanation of how that works.

We will do most of our coursework in Python, so before going on, make sure you're on Python 3.10 or 3.11 by downloading it from [https://www.python.org](https://www.python.org/). Later versions should work, but please upgrade if you are on an earlier version. Python 3.9 or below will not run the course software (3.8 and 3.9 are fine for the first few weeks).

Next open up the Terminal (Mac) or Command Line (PC) and install the Jupyter notebook with this command:

`pip install jupyter`

After that, go ahead and install music21 with:

`pip install music21`

You will need music21 v.8.1 or higher to complete this class. (If you have an earlier version, then `pip install --upgrade music21` will bring you up to date).

You might as well install Scientific Extensions to Python and the Levenshtein library for computing similarity while you're in installation mode. They're not absolutely needed for this class (so don't panic if they fail), but they will speed up working in music21:

`pip install scipy`  
`pip install python-Levenshtein`

Now you're ready to download the next part of the assignment: download the Jupyter notebook below and start learning and playing with the Jupyter environment. Save the notebook to a directory so that you know where it is. 

Change Directory in the terminal to that directory and run:

`jupyter notebook`

To start Jupyter. 

Then click on the file below and continue from here.

Download {{% resource_link "24f7e8ad-c277-4653-a6c3-49c2c40d0b2e" "mit21m.383s23\_class\_03\_lab\_02.ipynb;" %}} find it in Jupyter, read it, and make sure it works.