# SSPIV-dataset-for-turbulence-modelling
# Water Tunnel SSPIV and RANS Dataset

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19047404.svg)](https://doi.org/10.5281/zenodo.19047404)

** You can download this dataset from this link: [https://doi.org/10.5281/zenodo.19047404](https://doi.org/10.5281/zenodo.19047404) **

---

## 1. Overview
This repository contains high-resolution flow field measurements obtained using Stereoscopic Particle Image Velocimetry (SSPIV) in a water tunnel facility, alongside corresponding RANS simulation data and machine learning examples. The data provides detailed insights into the mean flow characteristics and turbulence structures.

## 2. Experimental Setup
* **Facility:** Water Tunnel
* **Measurement Technique:** Stereoscopic PIV (SSPIV)
* **Spatial Resolution:** 2 mm
* **Data Variables:** Time-averaged flow fields (`U`, `V`, `W`) and fluctuation statistics (RMS velocities and Reynolds stresses).

*(Please refer to the `Experimental Setup.png` file in the repository for a visual illustration of the experimental arrangement.)*

## 3. Directory Structure & File Descriptions

```text
📦 Repository Root
 ┣ 📂 Example/               # Machine learning demonstration
 ┃ ┣ 📂 dataset/             # Pre-processed .numpy data files for training
 ┃ ┗ 📜 TBNN.py              # Python script to train the Tensor Basis Neural Network
 ┣ 📂 RANS/                  # Computational Fluid Dynamics (CFD) results
 ┃ ┗ 📜 ...                  # OpenFOAM simulation results for the first 12 cases
 ┣ 📂 SSPIV/                 # Experimental SSPIV results
 ┃ ┣ 📜 Case_01.dat          # Contains spatial coordinates, mean flows, and statistics
 ┃ ┣ 📜 ...                  # Total of 36 .dat files for all experimental cases
 ┃ ┗ 📜 Case_36.dat
 ┣ 🖼️ Experimental Setup.png # Diagram of the experimental setup
 ┣ 📊 Index.xlsx             # Detailed working conditions and parameters for the 36 cases
 ┗ 📜 README.md              # This documentation file
