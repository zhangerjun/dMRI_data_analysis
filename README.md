# Mini-Project 5: Evaluation of Neonatal Brain Tissue Development Using Diffusion MRI

Team: Sara Hernandez, Kylie Xu, and Erjun Zhang (Mentor)

This mini-project was  completed by my two summer internship students, Kylie Xu and Sara Hernandez, at NeuroPoly in University De Montreal (POLY) and Magic lab in TransMedTech Institute in CHU Sainte Justine Hospital in summer 2023 (from June 02, 2023 to August 15, 2023). It is part of the project *An Introduction to Python-based MRI Data Analysis*.

## Introduction
While we do dMRI analysis, registration is a necessary and important step. Normally, researchers treat dMRI images as the other type of MR images and do the registration. While DTITK used diffusion tensor information to do the registration and it takes advantage of diffusion tensor information. 

As my knowledge, it is hard to find clear and complete steps to use it. Thus, this mini-project is trying to provide a easier way to use it (build the template, then do the registration), which could be interested by dMRI reserachers. Students can also use it as tutorial for excerise. 

## Goal
* Build the tempalte by using $71$ dHCP baby dti data;
* Registered these $71$ other babies to the template;
* Transfer the registration to the subject space.

## Methods

### Dataset
Data used in this project is 15 dHCP baby dMRI data. It can be [download here](http://www.developingconnectome.org/data-release/second-data-release/). Generally, these babies' averaged age is $39\pm0.5$ weeks. Baby list and information can be found in the folder Document and with file name [baby_list](https://github.com/zhangerjun/DTI-TK-Build-Template/blob/main/Document/baby_list.xlsx). 

### Some interesting experiment

## Results
![Results](./images/Result_figure_1.png)
## Reproducibility
### Dependencies
All the experiments can be completed online using either Windows, Mac or Linux computer.
* [Python 3](https://dti-tk.sourceforge.net/pmwiki/pmwiki.php?n=Main.HomePage), [Google colab notebooks](https://colab.research.google.com/) (or [Jupyter notebook](https://jupyter.org/))

* [DIPY](https://dipy.org/): nifti file loader and saver;
* Matplotlib, ipython widgets: data visualization;
* Useful tools: [ITK-SNAP](http://www.itksnap.org/pmwiki/pmwiki.php) for viewing nifti files locally, fsl-bet for creating human brain masks.

### Diliveries
* [Summary of the project](./documents/MiniProject_5_Summary_of_project.pdf): a brife discription of this project; We used this document for the mentorship project application;
* [Final report](./documents/MiniProject_5_Report.pdf): including all details of this project;
* [Project progress records](./documents/Progress_records_of_the_project.pdf): the every working day taskes were recorded for people, who want to reproduce the projects, to folow by themselves.
* [Slides](./documents/MiniProject_5_Slides_at_CHUSJ.pdf), [final presentation](./documents/MiniProject_5_Presentation_at_CHUSJ.mp4), [Abstract 1](./documents/MiniProject_5_abstract1.pdf), [Poster 1](./documents/MiniProject_5_poster1.pdf).


## Conclusion
We successfully reached our goal: use DTITK to build diffusion template;

*Acknowledgement*

We extend our sincere gratitude to QBIN for their invaluable financial support for this mini-project. Furthermore, we would like to express our deep appreciation to Dawson College (particularly Dr. Hélène Nadeau and Dr. Sylvia Cox) for providing us with the opportunity to collaborate and successfully bring this project to fruition. Our heartfelt thanks also go out to TransMedTech for generously providing us with a conducive and comfortable working environment. We also would like to thank Michelle Poulin for her assitant in this summer project; Finally, we would like to thank our supervisor Dr. De Leener, and Dr. Lodygensky for their supports throughout this project.


