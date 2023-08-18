# Mini-Project 5: Neonatal Brain Tissue Development Evaluation Using Diffusion MRI
(An Introduction to Python-based Medical Image Analysis) (in progress...)

Team: Sara Hernandez, Kylie Xu, and Erjun Zhang (Mentor)

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

## Reproducibility
### Dependencies
All the experiments can be completed online using either Windows, Mac or Linux computer.
* [Python 3](https://dti-tk.sourceforge.net/pmwiki/pmwiki.php?n=Main.HomePage), [Google colab notebooks](https://colab.research.google.com/) (or [Jupyter notebook](https://jupyter.org/))

* [DIPY](https://dipy.org/): nifti file loader and saver;
* Matplotlib, ipython widgets: data visualization;
* Useful tools: [ITK-SNAP](http://www.itksnap.org/pmwiki/pmwiki.php) for viewing nifti files locally, fsl-bet for creating human brain masks.

### Diliveries
* Project summary document: a brife discription of this project; We used this document for the mentorship project application;  
* Project final report (see in folder of document): including all details of this project;
* Project progress record (see in folder of document): the every working day taskes were recorded for people, who want to reproduce the projects, to folow by themselves.


## Conclusion
We successfully reached our goal: use DTITK to build diffusion template;

*Acknowledgement*

We extend our sincere gratitude to QBIN for their invaluable financial support for this mini-project. Furthermore, we would like to express our deep appreciation to Dawson College (particularly Dr. Hélène Nadeau and Dr. Sylvia Cox) for providing us with the opportunity to collaborate and successfully bring this project to fruition. Our heartfelt thanks also go out to TransMedTech for generously providing us with a conducive and comfortable working environment. We also would like to thank Michelle Poulin for her assitant in this summer project; Finally, we would like to thank our supervisor Dr. Benjamin De Leener, and Dr. Lodygensky for supports throughout this project.

This work was completed in NeuroPoly in University De Montreal (POLY) and Magic lab in TransMedTech Institute in CHU Sainte Justine Hospital.
In the future, some small experiments will be added (expect to complete by the end of Dec. 2023). 
