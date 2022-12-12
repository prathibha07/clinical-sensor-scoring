# <img src= "doc/electromyography.png" height="60"></img> Sensor Based Clinical Evaluations (SenBaCE)
---
[![Python Package using Conda](https://github.com/hanbincho/clinical-sensor-scoring/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/hanbincho/clinical-sensor-scoring/actions/workflows/python-package-conda.yml)

Analyze sensor activity from motor-impaired individuals to determine clinically relevant scores. Provide a quantitative evaluation of the impaired conditions, and to properly inform the rehabilitative process. 

## ToDo
Repository structure
* Use tree to generate this in the command line, screenshot, then attach image here. 

### Introduction
**SenBaCE** is a tool that aims to assign clinically relevant scores based off of plots created from sensor data collected during motor tasks from individuals with motor impairments. This tool can be used for score prediction based off the [U-Limb](https://academic.oup.com/gigascience/article/10/6/giab043/6304920) dataset and training with custom data.

**Dataset** U-Limb is a large, multimodal, multi-center dataset on human upper-limb movements. The kinematic data consists the position data of thorax, upper-and forearm markers. We are currently using the markers for thumb and little finger side
[Data] {https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/FU3QZ9} 



### Purpose
Currently, there are standard clinical practices where trained physicians visually assess motor impairments of patients. Based off these visual assessments, these physicians will then assign a score, which describes the severity of patients' impairments. To minimize possible biases or inconsistencies between assessments, sensor data can be utilized as a more robust and consistent means to characterize motor behaviors. However, the outputs of sensor data are not clinically meaningful and somewhat difficult to understand without additional filtering and processing. By utilizing a publicly available dataset that has collected sensor data and the corresponding clinical evaluation scores (U-Limb), and machine learning model techniques, **SenBaCE** aims to bridge this gap and demonstrate a potentially more robust alternative to clinically characterizing motor impairments.

### Installation and how to use
* Open a terminal and change your working directory to the desired location for the **SenBaCE** package.
* Clone the repoistory using `git clone https://github.com/hanbincho/clinical-sensor-scoring.git`
* `cd` into the repository `cd clinical-sensor-scoring`.
* Set up a new virtual environment with all necessary packages and their dependencies using `conda env create -f environment.yml`.
* Activate the virtual environment with `conda activate senbace`.
* `cd` into `senbace` package in the terminal via `cd senbace`
* In the terminal run `Streamlit run main.py --server.maxUploadSize 400`

---
SenBaCE logo adopted from [Icon8](https://icons8.com/icons/set/Electromyograph).

