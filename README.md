# **Placenta NMR Imaging - 1.5T vs 3.0T Study**
This repository contains code, reports, and a presentation related to the study of placental diffusion and perfusion using NMR imaging. The research compares acquisitions at 1.5T and 3.0T to analyze differences in diffusion and perfusion parameters between fetal and maternal regions of the placenta.

This repository contains code, reports, and a presentation related to the study of **placental diffusion and perfusion using NMR imaging**. The research compares acquisitions at **1.5T and 3.0T** to analyze differences in **diffusion and perfusion parameters** between fetal and maternal regions of the placenta.  

The project employs **advanced fitting models**, including:
- **Monoexponential Model**
- **IVIM (Intravoxel Incoherent Motion) Model**
- **Two-Compartment Perfusion Model**  

### **Project Description**
This repository contains **Python scripts, a scientific report, and a presentation** related to the **study of diffusion and perfusion in the human placenta using Nuclear Magnetic Resonance (NMR) imaging**.  

The research investigates whether **the results obtained by Maiuro et al.** in diffusion and perfusion studies depend on the strength of the **static magnetic field (1.5T vs. 3.0T)**. The study analyzes:
- **15 placentas scanned with a 1.5T Siemens Avanto scanner**
- **7 placentas scanned with a 3.0T Siemens Prisma scanner**

Three different mathematical models are applied to estimate diffusion and perfusion parameters:
1. **Monoexponential Model**  
2. **IVIM (Intravoxel Incoherent Motion) Model**  
3. **Two-Compartment Perfusion Model**  

---

## **Repository Contents**
### **📂 Python Scripts**
- **`1_5t_study.py`**  
  - Loads and processes **NIfTI images** acquired at **1.5T**.
  - Segments **fetal and maternal regions** of the placenta.
  - Generates **heatmaps** for diffusion and perfusion parameters.
  - Performs **statistical fitting** using Akaike Information Criterion (AIC).
  - Evaluates the **Signal-to-Noise Ratio (SNR)**.

- **`3t_study.py`**  
  - Loads and processes **NIfTI images** acquired at **3.0T**.
  - Performs **segmentation** and ROI (Region of Interest) analysis.
  - Applies **IVIM and Two-Compartment Perfusion Models** to fit the data.
  - Compares **fitting results across different field strengths**.
  - Generates **visual heatmaps** for parameter distributions.

### **📂 Documentation**
- **`Report_LAB_Belli_Contarini_1916927.pdf`**  
  - Detailed **scientific report** covering:
    - NMR theoretical background applied to placenta imaging.
    - **Preprocessing and segmentation** of placental images.
    - **Analysis of 1.5T vs. 3.0T imaging results**.
    - **Statistical validation**: Kolmogorov-Smirnov test, Welch’s t-test.
    - **Final conclusions** on diffusion and perfusion differences.

- **`Presentazione_LAB.pptx`**  
  - **Presentation slides** summarizing:
    - Basic definitions and research objectives.
    - Theoretical models applied.
    - Image segmentation and **SNR analysis**.
    - **Key results and statistical findings**.
    - **Final conclusions and future perspectives**.

---

## **Requirements**
To run the Python scripts, install the required dependencies:

```bash
pip install dipy nibabel numpy scipy matplotlib pandas tabulate
```

---

## **How to Run**
1. **Place the NIfTI files** in the appropriate folder.
2. **Run `1_5t_study.py`** to analyze placental imaging at **1.5T**.
3. **Run `3t_study.py`** to process and analyze images at **3.0T**.
4. **Review the results**:
   - Heatmaps of diffusion/perfusion parameters.
   - Statistical comparisons between **1.5T and 3.0T**.
   - Fitted model parameters and **goodness-of-fit tests**.

---

## **Authors**
- **Andrea Belli Contarini** (Student)
- **Silvia Capuani** (Tutor)
- 
Department of Physics, University of Rome "La Sapienza"  
Academic Year 2023-24

---

## **References**
1. **Maiuro et al.** (2023). *Two-compartment perfusion MR IVIM model to investigate normal and pathological placental tissue*. Journal of Magnetic Resonance Imaging.
2. **Callaghan, P. T.** (1993). *Principles of Nuclear Magnetic Resonance Microscopy*. Oxford University Press.

---

📌 **Note:** This repository is intended for academic research and methodology sharing in placental imaging using MRI.
