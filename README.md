# CORD-19-Qlik
A Qlik solution for the COVID-19 Open Research Dataset Challenge (CORD-19)

## Table of Contents

- [Introduction](#introduction)
    - [Demonstration Video](#demonstration-video)
- [Qlik Sense App](#qlik-sense-app)
- [Approach](#approach)

## Introduction
The [COVID-19 Open Research Dataset (CORD-19)](https://www.semanticscholar.org/cord19) is a growing resource of scientific papers on COVID-19 and related historical coronavirus research. A [Kaggle challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge) has been issued for this dataset, calling on the AI and Data Science community to develop tools that can help the medical community find answers to high priority scientific questions. 

COVID-19 research is [growing at an incredible rate](https://www.sciencemag.org/news/2020/05/scientists-are-drowning-covid-19-papers-can-new-tools-keep-them-afloat) and machine intelligence could be crucuial to help find insights in this repository of data.

This repository provides a Qlik Sense app for the CORD-19 dataset. The app combines the native search, navigation and interactive capabilities of Qlik Sense, with ML capabilities like Named Entity Recognition and Clustering. It also provides an automated load process for keeping the app up to date with new research that is being added to the CORD-19 dataset on a weekly basis.

### Demonstration Video
This short video provides a demonstration of the solution:

[!YouTube-Thumb](https://youtu.be/5fYWgglx84M)

## Qlik Sense App
The Qlik Sense app can be downloaded [here](app/CORD-19-Challenge.qvf). 

A reload of the app requires configuration of the data connections and the QVD files provided [here](data). It also requires the [PyTools Server Side Extension](https://github.com/nabeel-oz/qlik-py-tools). 

The app loads the JSON files for the research papers using Qlik's native REST connector. So a HTTP server hosting these files needs to be prepared and configured in the `Main` section of the app's load script.

## Approach
Work in progress.

