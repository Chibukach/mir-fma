---
title: 'Music Information Retrieval on FMA'
author:
- Michaël Defferrard^1^
include-before: ^1^ LTS2, EPFL, Switzerland
date: \today
numbersections: true
lang: en
---

# Administration

* People involved
	* Student: Chibueze Ukachi, \texttt{chibueze.ukachi@epfl.ch}
	* Supervisor: Michaël Defferrard, \texttt{michael.defferrard@epfl.ch}
	* Professor: Pierre Vandergheynst, \texttt{pierre.vandergheynst@epfl.ch}
* Amount of work: 10 ECTS (1/3 of a semester)
* Evaluation: A Jupyter notebook which explains (i) the problematic, (ii) the
  solution and, (iii) the results. Produced at the end of the project, no
  presentation required.
* Meeting of ~1h every week
* Repository: <https://lts2.epfl.ch/gitlab/michael.defferrard/fma-baselines>
	* Every file produced during the project should be in there.
* Dataset: Free Music Archive
	* Code & data: <https://github.com/mdeff/fma>
	* Paper: <https://arxiv.org/abs/1612.01840>
* The results obtained during this project will hopefully be integrated in the above paper.
	* ISMIR paper deadline: abstract April 21, full paper April 28

# Goal

The goal of this semester project is to provide baselines for genre
classification, and maybe other problems in Music Information Retrieval (MIR)
if time allows, on the [FMA dataset](https://github.com/mdeff/fma). We will
first test simple ML algorithms then devise and test Deep Networks. The idea is
to show that the dataset is large enough for end-to-end learning, i.e. from the
raw audio, with current DL techniques. This task involves the use of Python,
the Jupyter notebook and libraries such as scikit-learn and Keras (TensorFlow
backend).

## Plan

1. Try simple classifiers from scikit-learn.
	* Play with the dataset.
	* Get a sense of how difficult the problem is.
	* Learn about ML.
1. Implement a first simple fully connected feed-forward NN.
	* Learn Keras and see how NN works.
1. Find state-of-the-art DL and non-DL methods for MIR from raw audio.
1. Implement more convoluted models.
	* 1D CNNs on raw waveforms.
	* 2D CNNs on spectrograms.
	* RNNs: LSTMs, GRUs.
1. Eventually compare with echonest features.
1. Iterate and incrementally increase accuracy.

# Meetings

## 2017-02-07 (email)

Become familiar with Deep Learning. You won't need an in-depth knowledge to
work on the project, but an understanding of what is going on will be
necessary. Good resources are:

* this very complete book: <http://www.deeplearningbook.org/>
* or this course: <http://cs231n.github.io/>
* or this MOOC: <https://www.coursera.org/learn/neural-networks>

You may also want to look at the Keras library: <https://keras.io/>

## 2017-02-14

Discussed

* Find a place in lab, ask Rosie for accreditation
* Links: GitHub, paper
* Fix day and time to meet
* Chibu knows about scikit-learn, git, Jupyter, and ML from ADA
* Will have to learn Keras and Deep Learning
* git repository on gitlab
* no machine with GPU, we'll make an account on the CDK

For next week

* Register on IS-Academia
* Find a meeting time
* Clone the GitHub repository
* Import *fma_small* meta-data with pandas and explore the dataset
* Load and listen to audio clips from Python
* If time allows, try a linear regression with sklearn for genre recognition
