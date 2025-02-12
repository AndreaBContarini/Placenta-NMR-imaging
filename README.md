# **Placenta NMR Imaging - 1.5T vs 3.0T Study**
This repository contains code, reports, and a presentation related to the study of placental diffusion and perfusion using NMR imaging. The research compares acquisitions at 1.5T and 3.0T to analyze differences in diffusion and perfusion parameters between fetal and maternal regions of the placenta.

This repository contains code, reports, and a presentation related to the study of **placental diffusion and perfusion using NMR imaging**. The research compares acquisitions at **1.5T and 3.0T** to analyze differences in **diffusion and perfusion parameters** between fetal and maternal regions of the placenta.  

The project employs **advanced fitting models**, including:
- **Monoexponential Model**
- **IVIM (Intravoxel Incoherent Motion) Model**
- **Two-Compartment Perfusion Model**  

The code processes **NIfTI medical images**, performs **segmentation**, generates **heatmaps**, and applies **statistical model selection techniques** like Akaike Information Criterion (AIC).  

📌 **This repository provides Python scripts, a detailed report, and a presentation summarizing the results of the study.**  


### **Project Description**
This repository contains Python code, a scientific report, and a presentation related to the **study of diffusion and perfusion in the human placenta using Nuclear Magnetic Resonance (NMR) imaging**.  

The research aims to determine whether the **results obtained by Maiuro et al.** in diffusion and perfusion studies depend on the strength of the **static magnetic field (1.5T vs. 3.0T)**. The study analyzes:
- **15 placentas scanned with a 1.5T Siemens Avanto scanner**
- **7 placentas scanned with a 3.0T Siemens Prisma scanner**

Three different mathematical models are applied to estimate diffusion and perfusion parameters:
1. **Monoexponential Model**  
2. **IVIM (Intravoxel Incoherent Motion) Model**  
3. **Two-Compartment Perfusion Model**  

---

## **Repository Contents**
📂 **`1_5t_study.py`**  
A Python script for:
- **Loading and preprocessing NIfTI images**
- **Segmenting fetal and maternal regions of interest (ROI)**
- **Generating heatmaps for diffusion and perfusion parameters**
- **Fitting models and calculating Akaike Information Criterion (AIC)**
- **Analyzing Signal-to-Noise Ratio (SNR)**

📂 **`Report_LAB_Belli_Contarini_1916927.pdf`**  
A detailed scientific report covering:
- Theoretical background of NMR and placental imaging
- Data acquisition and preprocessing steps
- Analysis of 1.5T vs. 3.0T imaging results
- Statistical comparisons, including **Kolmogorov-Smirnov test and Welch’s t-test**
- Final conclusions on model effectiveness

📂 **`Presentazione_LAB.pptx`**  
Presentation slides summarizing:
- Basic definitions and research objectives
- Theoretical models used in the study
- Image segmentation and SNR analysis
- Key results and statistical validation
- Final conclusions and discussion

---

## **Requirements**
To run **`1_5t_study.py`**, install the necessary dependencies:

```bash
pip install dipy nibabel numpy scipy matplotlib
```
---

## **How to Run**
1. **Place the NIfTI files** in the correct folder
2. **Run the Python script** to generate heatmaps and extract diffusion/perfusion parameters
3. **Refer to the PDF report** for result interpretation
4. **Use the PowerPoint presentation** for a quick overview of the findings

---

## **Authors**
- **Andrea Belli Contarini** (Student)
- **Silvia Capuani** (Tutor)

Department of Physics, University of Rome "La Sapienza"  
Academic Year 2023-24

---

## **References**
1. **Maiuro et al.** (2023). *Two-compartment perfusion MR IVIM model to investigate normal and pathological placental tissue*. Journal of Magnetic Resonance Imaging.
2. **Callaghan, P. T.** (1993). *Principles of Nuclear Magnetic Resonance Microscopy*. Oxford University Press.

---

📌 **Note:** This repository is intended for academic research and methodology sharing in placental imaging using MRI.

