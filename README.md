# Mini-Project 5: Neonatal Brain Tissue Development Evaluation Using Diffusion MRI
(An Introduction to Python-based Medical Image Analysis) (in progress...)

Team: Sara Hernandez, Kylie Xu, Erjun Zhang (Mentor)

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





### Build template


### Register subjects to template
#### Generate the path to template
#### Registration

The maps after registration is named: ${subject name}+map_type+'commbined'+'.nii.gz'
### Some interesting experiment
## Results & Discussion
* Template generated
<div align="left">
	<img src="./figure/template_rgb.png" width="500" alt="1" title="template created (rgb map)">
</div>

The template file can be found in the folder template. Figures of this file can also be found there.

* Registered files

<div align="left">
	<img src="./figure/fa_after_registration.gif" width="300" alt="1" title="FA after registration">
</div>

* Experiment results

## Reproducibility
### Dependencies
* [DTITK software](https://dti-tk.sourceforge.net/pmwiki/pmwiki.php?n=Main.HomePage);
* [itksnap](http://www.itksnap.org/pmwiki/pmwiki.php): nifti file viewer;
* [DIPY](https://dipy.org/): nifti file loader and saver;
* matplotlib, plotly and ipython widgets: data visualization;
* Linux (Ubuntu 22.04);
* Other python libaries.
### Usage
For template generatation and registration, 
1. Download dHCP second dataset (you can only download the dMRI dataset) to your local computer;
2. Download this code and put it somewhere;
3. Then, generate template and register:
	* Following its ipynb file (for example, *dtitk_registration_dhcp.ipynb* for registration. 
	* If you see run shell script,
		* First copy brain name list in *subj.txt* to the specific files;
		* Then run specific *#.sh* files.
4. The template and registration files will be stored in the folder *template* and *template_reg*. The generated template file is named *template_final.nii.gz*; The registered maps were named *averaged_maptype.nii*.

**Notes** 

* Generating template should be first done before registration, unless you have the tensor template aready.
* If you are interested in build template with *dti_template_bootstrap*, you can copy the *./figure/template_final.nii.gz* to folder *template*, rename it as *template_for_bootstrap.nii.gz*; run *built_template_bootstrap.sh*.
* If you use group command, at least $2$ subjects should be added.
* The first line of builtTemp.sh and Template_reg.sh may cause automatically run failly. It can be commanded out. 
* DTITK will make the origin (-0,-0,-0), this will cause problem while the origin of original tk file is (0,0,0). Editing the template origin to (0,0,0) can solve this problem.
* 
## Conclusion
We successfully reached our goal: use DTITK to build diffusion template;

Deliverables:
* **dhcp_data_list.ipynb**: grab baby information from downloaded dhcp dataset;
* **dtitk_template_dhcp.ipynb**: code for generating template and virulization;
* **dtitk_registration_dhcp.ipynb**: code for registration and visulization of registration.



*Acknowledgement*

We wanted to acknowledge our mentor Erjun Zhang for helping us along the way and teaching us the basis of
python coding and medical-imaging. This project would have been impossible to complete without his help. In addition,
we wanted to thank our Dawson College supervisors, Dr. Hélène Nadeau and Dr. Sylvia Cox for giving us feedback on
our project. And finally, we wanted to acknowledge Michelle Poulin, Dr. Benjamin De Leener and Dr. Lodygensky for
helping us and taking care of us in the hospital during our internship.

This work was completed in NeuroPoly in University De Montreal (POLY) and Magic lab in TransMedTech Institute in CHU Sainte Justine Hospital. I would like to thanks CHU Saint Justine ...

In the future, some small experiments will be added (expect by the end of Dec. 2023). 
